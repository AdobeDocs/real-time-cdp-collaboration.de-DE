---
title: Konfigurieren von AWS-Berechtigungen für die Zielgruppen-Beschaffung
description: Erfahren Sie, wie Sie Berechtigungen für die Identitäts- und Zugriffsverwaltung (IAM) von AWS konfigurieren, um Adobe für die Zielgruppen-Beschaffung in Real-Time CDP Collaboration sicheren, schreibgeschützten Zugriff auf Ihren  [!DNL Amazon S3]  zu gewähren.
source-git-commit: 73f11b7341cf94540dc01f8803291f6dc3cd5038
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 1%

---

# Konfigurieren von AWS-Berechtigungen für die Zielgruppen-Beschaffung

Verwenden Sie dieses Handbuch, um AWS Identity and Access Management (IAM)-Richtlinien und -Rollen zu konfigurieren, die Adobe sicheren, schreibgeschützten Zugriff auf Ihren Amazon S3-Bucket gewähren. Dieser Zugriff ermöglicht es Real-Time CDP Collaboration, Zielgruppen aus Ihrem S3-Bucket zu beziehen.

## Voraussetzungen {#prerequisites}

Bevor Sie fortfahren, vergewissern Sie sich, dass Sie die folgenden Anforderungen erfüllen und Zugriff auf die erforderlichen Informationen haben.

### Erforderliche AWS-Berechtigungen

Um diese Einrichtung abzuschließen, muss Ihr Konto über Administratorrechte für AWS verfügen. Der Administratorzugriff stellt sicher, dass Sie IAM-Richtlinien und -Rollen erstellen und verwalten können, die erforderlich sind, um den Zugriff von Adobe auf Ihren S3-Bucket zu autorisieren. Wenn Sie keine Administratorrechte haben, wenden Sie sich an Ihren AWS-Administrator, bevor Sie fortfahren.

### Erforderliche Informationen

Notieren Sie sich die folgenden Informationen, wenn Sie die folgenden Schritte durchlaufen. Diese Details werden im Handbuch zur [[!DNL Amazon S3] -Benutzeroberfläche verwendet](./configure-aws-s3-audience-sourcing.md).

* Der S3-Behältername, in dem Ihre Zielgruppendateien gespeichert werden.
* Der Ordnerpfad (Präfix), unter dem sich Ihre Zielgruppendateien befinden.
* Der Amazon-Ressourcenname (ARN) für Ihre neu erstellte IAM-Rolle, z. B.: `arn:aws:s3:::my-company-data/audience-files/`

>[!TIP]
>
>Ein Amazon Resource Name (ARN) identifiziert AWS-Ressourcen, wie z. B. S3-Buckets und IAM-Rollen, eindeutig. Verwenden Sie das folgende Format, um Ihren -Behälter und den optionalen Ordnerpfad anzugeben:
>
>```
>arn:aws:s3:::<bucket-name>/<optional-folder-path>
>```

## Erstellen einer IAM-Richtlinie {#create-policy}

Erstellen Sie zunächst eine IAM-Richtlinie, die Ihrem S3-Bucket **schreibgeschützten Zugriff** gewährt. Diese Richtlinie ermöglicht Adobe das Lesen der für die Zielgruppen-Beschaffung erforderlichen Dateien, gewährt jedoch keine Schreib- oder Löschberechtigungen.

Öffnen Sie die [AWS-Verwaltungskonsole](https://aws.amazon.com/console/) und navigieren Sie zu **[!DNL IAM]** > **[!DNL Policies]** > **[!DNL Create policy]**.

Wählen Sie im Arbeitsbereich Richtlinie erstellen in AWS die Registerkarte **JSON** und fügen Sie die folgende Beispielrichtlinie ein.

>[!NOTE]
>
>Ersetzen Sie `<Your AWS ARN for bucket folder path>` und `<Your AWS ARN for bucket>` durch Ihre spezifischen S3-ARNs. Wenn Sie den Pfad des Bucket-Ordners angeben, fügen Sie `/*` am Ende des ARN ein (z. B. `arn:aws:s3:::my-company-data/audience-files/*`). Dadurch wird sichergestellt, dass Adobe Zugriff auf alle Dateien und Unterordner innerhalb des angegebenen Ordnerpfads hat.

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Action": [
        "s3:GetObject",
        "s3:ListBucket",
        "s3:GetBucketLocation"
      ],
      "Resource": "<Your AWS ARN for bucket folder path>"
    },
    {
      "Sid": "Statement2",
      "Effect": "Allow",
      "Action": [
        "s3:ListBucket"
      ],
      "Resource": "<Your AWS ARN for bucket>"
    }
  ]
}
```

Überprüfen Sie die Richtlinieneinstellungen und wählen Sie **[!DNL Create policy]** aus. Notieren Sie sich den Richtliniennamen zur Verwendung in einem späteren Schritt.

>[!TIP]
>
>Um Ihren Behälternamen und Ordnerpfad zu finden, öffnen Sie die **Amazon S3-Verwaltungskonsole**. Wählen Sie auf der **Buckets**-Seite Ihren Bucket-Namen aus, um ihn zu öffnen. Die **Objekte**-Ansicht listet Ihre Dateien und Ordner auf, und der Pfad oben auf der Seite zeigt Ihren aktuellen Ordnerpfad an.

## Erstellen einer IAM-Rolle {#create-role}

Erstellen Sie anschließend eine IAM-Rolle und legen Sie die IAM-Rolle von Real-Time CDP Collaboration AWS als **vertrauenswürdige Entität“**. Dadurch können die Services von Adobe die Rolle übernehmen und Ihre S3-Zielgruppendaten sicher lesen.

Navigieren Sie in der Amazon S3 Management Console auf der Registerkarte **[!DNL IAM]** zu **[!DNL Roles]** > **[!DNL Create role]**.

Wählen Sie unter [!DNL Step 1] des [!DNL Create role]-Workflows im Abschnitt **[!DNL Trusted entity type]** die Option **[!DNL Custom trust policy]** aus. Fügen Sie dann im **[!DNL Custom trust policy]**-Editor das folgende Beispiel ein und ersetzen Sie `<Adobe IAM Role ARN>` durch den Wert für Ihre Region.

* Die entsprechende Adobe IAM-Rolle für ARN für Ihre Region:

| Region | Adobe IAM Role ARN |
|---------|-------------------|
| Nordamerika | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-va6-role` |
| Australien | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-aus3-role` |
| EMEA | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-deu1-role` |

Ein Beispiel für eine Vertrauensrichtlinie:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Principal": {
        "AWS": "<Adobe IAM Role ARN>"
      },
      "Action": "sts:AssumeRole"
    }
  ]
}
```

Überprüfen Sie die Richtlinie und wählen Sie **Weiter**, um fortzufahren.

Suchen Sie [!DNL Step 2] Abschnitt **[!DNL Add permissions]** des [!DNL Create role]-Workflows nach der von Ihnen (zuvor[&#x200B; erstellten IAM-Richtlinie und fügen Sie sie &#x200B;](#create-policy). Wählen Sie die Richtlinie und anschließend **[!DNL Next]** aus, um fortzufahren[!DNL Step 3].

Geben Sie im Abschnitt [!DNL Step 3] **[!DNL Name review, and create - Role details]** einen Rollennamen (z. B. `s3-iam-role`) und eine optionale Beschreibung an.

Auf dieser Seite werden die Richtlinie für vertrauenswürdige Entitäten, die Zusammenfassung der Berechtigungsrichtlinien und alle Tags angezeigt, die Sie möglicherweise für die interne Organisation und Verfolgung hinzugefügt haben.

Wählen Sie abschließend **Rolle erstellen** aus, um die Einrichtung zu bestätigen.

>[!IMPORTANT]
>
>Sie müssen den Amazon-Ressourcennamen (ARN) aufzeichnen, nachdem Sie die Rolle erstellt haben. Sie müssen die IAM-Rollen-ARN während des Schritts **Authentifizieren Ihrer S3-Verbindung** im Workflow [Konfigurieren von AWS S3 für die &#x200B;](./configure-aws-s3-audience-sourcing.md)&quot; angeben.

## Nächste Schritte {#next-steps}

Dadurch erhält Adobe schreibgeschützten Zugriff auf Ihren S3-Bucket und eine vertrauenswürdige Verbindung mit der IAM-Rolle von Adobe.

Fahren Sie als Nächstes mit [Konfigurieren von AWS S3 für die Zielgruppen-Beschaffung](./configure-aws-s3-audience-sourcing.md) fort, um Ihren S3-Bucket mit Collaboration zu verbinden.

Weitere Informationen zum Abrufen von Zielgruppen finden Sie unter [Source und Verwalten von Zielgruppen](./onboard-audiences.md).
