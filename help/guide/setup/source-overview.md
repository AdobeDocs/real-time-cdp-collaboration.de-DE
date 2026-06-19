---
title: Quellen – Übersicht
description: Informationen zu Quell-Connectoren in Adobe Real-Time CDP Collaboration
audience: admin, publisher, advertiser
source-git-commit: b30d1b01e929e586404faac34650c7fd479d071b
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 6%

---

# Quellen – Übersicht

In Adobe Real-Time CDP Collaboration stammen Ihre Zielgruppendaten aus einer Quelle (oder Datenverbindung). Sie können eine Verbindung zu verschiedenen Quelltypen herstellen, z. B. zu Adobe-Programmen, Cloud-basierten Datenspeichern oder Dateien aus Ihrem lokalen System, um Zielgruppen für Ihre Collaboration[Projekte zu ](./onboard-audiences.md) und zu verwalten. Während des Zielgruppen-Beschaffungs-Workflows können Sie Ihre bevorzugte Quelle basierend auf den Anforderungen Ihres Unternehmens auswählen und einrichten.

## Mit Quelle verbinden {#connect-a-source}

Um eine Quelle zu verbinden, müssen Sie den Beschaffungs-Workflow eingeben. Navigieren Sie zunächst zur Registerkarte **[!UICONTROL Meine Zielgruppen]** im **[!UICONTROL Setup]**-Arbeitsbereich.

Wählen Sie das Symbol zum Hinzufügen aus ![Symbol hinzufügen.](/help/assets/icons/plus.png)) und wählen Sie dann **[!UICONTROL Audience]** aus, um den Quell-Workflow zu starten.

![Mein Zielgruppen-Arbeitsbereich mit hervorgehobener Option „Hinzufügen“ und hervorgehobener Option „Zielgruppen“.](/help/assets/setup/add-manage-audiences/add-audiences.png)

Während des Workflows werden Sie aufgefordert, eine neue Datenverbindung hinzuzufügen, indem Sie eine Quelle auswählen. Die ausgewählte Quelle bestimmt, wie Ihre Zielgruppendaten in Collaboration importiert werden. Eine Liste [ unterstützten Quellen finden Sie ](#available-sources) der Tabelle „Verfügbare Quellen“.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit hervorgehobener Option „Neue Datenverbindung hinzufügen“.](/help/assets/setup/add-manage-audiences/add-data-connection.png)

Nach der Auswahl einer Quelle führt Sie der Workflow durch die verbindungsspezifischen Setup-Schritte, einschließlich Authentifizierung, Feldzuordnung, Planung und Zielgruppenauswahl.

### Verfügbare Quellen {#available-sources}

Die folgenden Quellen sind in Collaboration verfügbar. Um die schrittweise Anleitung zur Beschaffung für diese Quelle anzuzeigen, wählen Sie den Namen der Quelle in der folgenden Tabelle aus. Wenn Sie an einer Quelle interessiert sind, die derzeit nicht verfügbar ist, wenden Sie sich an den Adobe-Support.

| Quelle | Beschreibung | Verfügbarkeit |
| --- | --- | --- |
| [Adobe Experience Platform](./onboard-audiences.md) | Binden Sie Zielgruppen aus Ihrer verbundenen Experience Platform-Instanz ein und verwenden Sie bestehende Kundensegmente wieder. | Verfügbar |
| [Amazon S3](./configure-aws-s3-audience-sourcing.md) | Verbinden Sie Ihre S3-Buckets, um große First-Party-Datensätze aus Ihrer Cloud-Infrastruktur zu beziehen. | Verfügbar |
| [[!DNL Snowflake]](./configure-snowflake-audience-sourcing.md) | Verbinden Sie Ihre [!DNL Snowflake Secure Data Share], um umfangreiche Zielgruppendaten aufzunehmen. | Verfügbar |
| [[!DNL Google Cloud Storage]](./configure-gcs-audience-sourcing.md) | Verbinden Sie Ihre GCS-Buckets, um in Ihrer [!DNL Google Cloud]-Umgebung gespeicherte Zielgruppendaten einzubringen. | Verfügbar |
| [CSV-Datei hochladen](./upload-csv-audience-sourcing.md) | Laden Sie eine formatierte CSV-Datei direkt von Ihrem lokalen System hoch. | Verfügbar |
| Adobe Audience Manager | Übertragen Sie vorhandene Audience Manager-Segmente in Ihre Collaboration-Projekte. | *Bald verfügbar* |
| [[!DNL Azure Blob Storage]](./configure-azure-storage-audience-sourcing.md) | Verbinden Sie Ihre [!DNL Azure Blob Storage]-Container mit Erstanbieter-Datensätzen aus Ihrer [!DNL Microsoft Azure]. | Verfügbar |
| [[!DNL Azure Data Lake Storage]](./configure-azure-storage-audience-sourcing.md) | Verbinden Sie Ihr [!DNL Azure Data Lake Storage Gen 2]-Konto, um Zielgruppendaten einzubringen, die in Ihrem [!DNL Azure] Data Lake gespeichert sind. | Verfügbar |

{style="table-layout:auto"}

## Nächste Schritte

Nachdem Sie eine Quelle verbunden und Ihre Zielgruppen eingebracht haben, können Sie Details anzeigen, Konfigurationen aktualisieren oder vorhandene Quellen löschen. Weitere Informationen finden Sie im [Datenverbindungen verwalten](./manage-data-connection.md).
