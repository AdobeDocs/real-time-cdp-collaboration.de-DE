---
title: Konfigurieren  [!DNL Amazon S3]  Zielgruppen-Beschaffung
description: Erfahren Sie, wie Sie Ihren - [!DNL Amazon S3]  als Self-Service-Datenquelle konfigurieren und verbinden können, um Zielgruppendaten in Real-Time CDP Collaboration aufzunehmen.
exl-id: 566ceb1b-a72a-413d-b07d-409723892616
source-git-commit: 43134d6f334ee500834a6451bdf1a8f7372f8d10
workflow-type: tm+mt
source-wordcount: '1583'
ht-degree: 1%

---

# Konfigurieren von [!DNL Amazon S3] für die Zielgruppen-Beschaffung

Erfahren Sie, wie Sie Ihren [!DNL Amazon S3] in der Benutzeroberfläche von Adobe Real-Time CDP Collaboration konfigurieren und verbinden, um Zielgruppendaten für Aktivierungs- und Überschneidungsanalysen zu beziehen.

>[!IMPORTANT]
>
>Bevor Sie dieses Handbuch befolgen, müssen Sie die Schritte ausgeführt haben, um die IAM-Rolle von Adobe in Ihrem AWS-Konto zu autorisieren.\
>Eine schrittweise Anleitung zur Einrichtung **[finden Sie](./configure-aws-permissions-audience-sourcing.md)** Handbuch Konfigurieren von AWS-Berechtigungen für die Zielgruppen-Beschaffung .

## Überblick {#overview}

Verwenden Sie diesen Workflow, um Erstanbieter-Zielgruppen direkt aus [!DNL Amazon S3] zu beziehen und zu verwalten. Nach der Konfiguration bezieht Collaboration Zielgruppen automatisch aus Ihrem S3-Bucket und stellt sie für Einblicke und Aktivierungen zur Verfügung.

Zielgruppen, die über S3 bezogen werden, folgen denselben Governance- und Datenverarbeitungsregeln wie die Zielgruppen, die über Adobe Experience Platform bezogen werden.

## Voraussetzungen {#prerequisites}

Stellen Sie vor dem Konfigurieren Ihrer S3-Datenverbindung Folgendes sicher:

* Sie haben Zugriff auf einen aktiven **[!DNL Amazon S3]-Bucket** der Zielgruppendateien enthält, die der **[Zielgruppen-Beschaffungsspezifikation (v1.1)](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf)**.
* Sie haben eine **IAM-Rolle** in AWS erstellt, die Adobe die Berechtigung zum Zugriff auf Ihren Bucket mithilfe der Methode **Angenommene Rolle** (keine Zugriffs-/Geheimschlüssel) gewährt. Detaillierte **[finden Sie unter „Konfigurieren von AWS](./configure-aws-permissions-audience-sourcing.md)** Berechtigungen für die Zielgruppen-Beschaffung“. Die IAM-Rolle muss die folgenden Berechtigungen enthalten:

   * `ListBucket`
   * `GetBucketLocation`
   * `GetObject`

* Sie haben die folgenden Werte bereit:

   * **IAM-Rolle Amazon Resource Name (ARN)**
   * **S3-Bucket-Name**
   * **Ordnerpfad** (das Ordnerpräfix, das Ihre Zielgruppendateien enthält)

>[!NOTE]
>
>Zielgruppendateien müssen sich im **Stammordnerpfad** Ihres autorisierten S3-Buckets befinden. Unterordnerstrukturen werden nicht unterstützt.

## Konfigurieren der [!DNL Amazon S3] {#configure-aws-s3-connection}

Wählen Sie im Arbeitsbereich **[!UICONTROL Setup]** **[!UICONTROL auf der Registerkarte „Meine Zielgruppen]** das Symbol zum Hinzufügen (![Hinzufügen) aus.](/help/assets/icons/plus.png)) und wählen Sie dann **[!UICONTROL Audience]** aus.

Wenn dies Ihre erste Zielgruppe ist, können Sie auch die Option **[!UICONTROL Hinzufügen]** auswählen.

![Die Registerkarte „Meine Zielgruppen“ im Arbeitsbereich „Setup“ mit dem Symbol „Hinzufügen“ und der Option „Zielgruppe hinzufügen“ wird angezeigt.](../../assets/setup/add-manage-audiences/add-audiences.png)

Der Workflow „Zielgruppe hinzufügen“ wird angezeigt. Wählen Sie **[!UICONTROL Neue Datenverbindung hinzufügen]** und dann **[!UICONTROL Weiter]** aus.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit hervorgehobener Option „Neue Datenverbindung hinzufügen“.](../../assets/setup/add-manage-audiences/add-data-connection.png){zoomable="yes"}

### [!DNL Amazon S3] als Datenverbindung auswählen {#select-aws-s3}

Wählen Sie **[!UICONTROL Amazon S3]** als Datenverbindung aus, gefolgt von **[!UICONTROL Weiter]**.

![Der Bildschirm zur Auswahl der Datenverbindung mit [!DNL Amazon S3] als auswählbare Option.](../../assets/setup/aws-audience-sourcing/select-s3-data-connection.png)

### Anforderungen an Zielgruppendateien überprüfen {#review-audience-requirements}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_audience_sourcing_specifications"
>title="Daten für das Onboarding vorbereiten"
>abstract="Lesen Sie das Handbuch zur Spezifikation von Audience Sourcing , um zu erfahren, wie Sie Zielgruppendaten aus Amazon S3 für Collaboration formatieren und strukturieren."
>additional-url="https://www.adobe.com/go/rtcdp-collaboration-audience-sourcing" text="Siehe Handbuch"

Es wird ein Dialogfeld angezeigt, in dem erläutert wird, wie Ihre Zielgruppendateien strukturiert sein müssen. Verwenden Sie den Link zur **[[!UICONTROL Zielgruppen-Beschaffungsspezifikation]](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf)**, um zu erfahren, wie Sie Zielgruppendaten aus [!DNL Amazon S3] formatieren und strukturieren, damit sie von Collaboration korrekt gelesen werden können.

>[!IMPORTANT]
>
>Sie müssen Adobe als [!DNL Amazon S3] Benutzer autorisiert haben, damit Adobe Daten aus Ihrem [!DNL Amazon S3] zur Verarbeitung abrufen kann.

Ihre Zielgruppendateien müssen der Zielgruppen-Beschaffungsspezifikation entsprechen. Die Übereinstimmungsschlüssel werden automatisch auf der Grundlage des erforderlichen Formats zugeordnet.

Zu den wichtigsten Aspekten gehören:

* Dateien müssen im CSV-Format sein und mehrere Werte durch Kommas als Trennzeichen und senkrechte Striche (`|`) voneinander trennen.
* Stellen Sie beim Hochladen mehrerer Dateien sicher, dass alle Dateien identische Spalten enthalten.
* Jeder Zielgruppen-Datensatz muss einen `AUDIENCE_ID` und mindestens einen Übereinstimmungsschlüssel enthalten, z. B. `HASHED_EMAIL_SHA_256`, `HASHED_PHONE_SHA_256`, `HASHED_IPV4_SHA_256`, `CRM_ID`, `LOYALTY_ID` oder `ADFIXUS_ID`.
* Datenaktualisierungen erfolgen alle 1-6 Tage basierend auf Ihrer Auswahl während der Einrichtung der Beschaffung in Collaboration.

![Das Dialogfeld „Daten für die Beschaffung vorbereiten“ mit einem Link zu den Spezifikationen für die Zielgruppenbeschaffung.](../../assets/setup/aws-audience-sourcing/prepare-data-sourcing-dialog.png)

### S3-Verbindung authentifizieren {#authenticate-s3-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_sources_s3_folderpath"
>title="Pfadformat des Ordners"
>abstract="Geben Sie den Ordnerpfad (Präfix) in Ihrem [!DNL Amazon S3] ein, in dem Ihre Zielgruppendateien gespeichert sind.<br><ul><li>Beginnen Sie Pfade nicht mit einem Schrägstrich (/).</li><li>Fügen Sie am Ende des Pfads einen Schrägstrich hinzu.</li><ul><br>Gültiges Beispiel: `base/path/`<br>Ungültiges Beispiel: `/base/path`"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_audience_sharing_amazon_s3"
>title="Zielgruppe für Amazon S3 hinzufügen"
>abstract="Um Ihren Amazon S3-Speicher zu verbinden, autorisieren Sie den Service-Benutzer von Adobe, Ihre Zielgruppendaten zur Verarbeitung abzurufen. Führen Sie die in Experience League beschriebenen Schritte aus, um Adobe Zugriff auf Ihren Amazon S3-Speicher zu gewähren."

Geben Sie als Nächstes Ihre [!DNL Amazon S3] Anmeldeinformationen ein, um Ihren S3-Bucket mit Collaboration zu verbinden.

Führen Sie die unter **[von AWS-Berechtigungen für Zielgruppen-Sourcing beschriebenen Schritte aus](./configure-aws-permissions-audience-sourcing.md)** um Adobe Zugriff auf Ihre zu gewähren.
[!DNL Amazon S3]. Geben Sie nach Abschluss des Vorgangs Ihre Werte in die folgenden Benutzeroberflächenfelder ein:

* IAM-Rolle
* S3-Bucketname
* Ordnerpfad

![Das [!DNL Amazon S3]-Verbindungsformular mit Feldern für die IAM-Rolle, den S3-Behälternamen und den Ordnerpfad.](../../assets/setup/aws-audience-sourcing/s3-authentication-credentials-form.png)

### Einverständnisbestätigung bestätigen {#confirm-consent}

Sie müssen dann bestätigen, dass die Einverständnis-Opt-outs entfernt wurden, bevor Sie fortfahren. Markieren Sie zur Bestätigung das Bestätigungsfeld **[!UICONTROL OK]**.

![Das Dialogfeld zur Bestätigung des Einverständnis-Opt-outs, das vor dem Fortfahren bestätigt werden muss.](../../assets/setup/aws-audience-sourcing/consent-optout-acknowledgment.png)

### Authentifizierungsergebnisse überprüfen {#validate-authentication}

Nach dem Verbinden validiert das System Ihre Anmeldeinformationen und zeigt eine der folgenden Meldungen an:

| Status | Nachricht | Beschreibung |
|---| ---|---|
| **Erfolg** | **[!UICONTROL Authentifizierung erfolgreich]** | Ihre Verbindung mit [!DNL Amazon S3] wurde erfolgreich hergestellt. |
| **Fehlgeschlagen** | **[!UICONTROL Authentifizierung fehlgeschlagen]** | Bitte überprüfen Sie Ihre Anmeldedaten und versuchen Sie es erneut. |
| **Zugriff verweigert** | **[!UICONTROL Zugriff verweigert]** | Ihre Anmeldedaten verfügen nicht über die erforderlichen Berechtigungen, um auf diesen [!DNL Amazon S3]-Bucket zuzugreifen. Überprüfen Sie die Zugriffseinstellungen oder wenden Sie sich an Ihren Administrator. |
| **Ungültiges Dateiformat** | **[!UICONTROL Ungültiges Dateiformat]** | Die Zielgruppendaten stimmen nicht mit der erwarteten Struktur überein. Stellen Sie sicher, dass Ihre Dateien den Spezifikationen für die Zielgruppenbeschaffung entsprechen. |
| **Keine Zielgruppendateien gefunden** | **[!UICONTROL Keine Zielgruppendateien gefunden]** | Bestätigen Sie, dass sich Ihre Zielgruppendateien im angegebenen Ordnerpfad befinden und dass auf den Pfad zugegriffen werden kann. |
| **Interner Fehler** | **[!UICONTROL Ein interner Fehler ist aufgetreten]** | Bitte erneut versuchen. Wenn das Problem weiterhin besteht, wenden Sie sich an den Support. |


### Angeben von Verbindungsdetails {#provide-connection-details}

Geben Sie einen beschreibenden Namen und eine optionale Beschreibung für Ihre S3-Datenverbindung ein. Geben Sie Ihre Werte in die folgenden Benutzeroberflächenfelder ein:

* **[!UICONTROL Name der Datenverbindung]** (erforderlich)
* **[!UICONTROL Beschreibung der Datenverbindung]** (optional)

![Das Formular mit den Datenverbindungsdetails mit Feldern für den Verbindungsnamen und die Beschreibung.](../../assets/setup/aws-audience-sourcing/s3-connection-name-description.png)

### Überprüfen der automatisch zugeordneten Identitätsfelder {#auto-mapped-fields}

Der **[!UICONTROL Zuordnung]** ist schreibgeschützt. Sie können keine Umwandlungen hinzufügen, löschen oder anwenden. Collaboration ordnet Quell-Identitätsfelder aus Ihren Zielgruppendateien basierend auf der Zielgruppen-Beschaffungsspezifikation automatisch Zielfeldern zu.

Bestätigen Sie die zugeordneten Felder visuell und wählen Sie **[!UICONTROL Weiter]** aus, um fortzufahren.

![Der Bildschirm für die Feldzuordnung mit automatisch zugeordneten Quell- und Ziel-Identitätsfeldern.](../../assets/setup/aws-audience-sourcing/s3-field-mapping-auto-mapped.png)

### Aktualisierungshäufigkeit und Datumsbereich planen {#schedule-refresh}

Die **[!UICONTROL Zeitplan]**-Ansicht wird angezeigt. Wählen Sie im Dropdown-Menü eine Aktualisierungshäufigkeit zwischen einem und sechs Tagen aus und legen Sie dann den aktiven Datumsbereich fest. Verwenden Sie das Kalendersymbol, um Start- und Enddatum anzugeben.

>[!IMPORTANT]
>
>Um Ihre Collaboration-Credits effektiv zu verwalten, legen Sie die Aktualisierungshäufigkeit so fest, dass sie mit der Aktualisierungshäufigkeit Ihrer zugrunde liegenden S3-Daten übereinstimmt oder diese überschreitet. Das unterstützte Mindestaktualisierungsintervall beträgt einmal alle sechs Tage.

![Der Bildschirm mit den Zeitplaneinstellungen mit den Optionen für die Aktualisierungshäufigkeit und der Konfiguration des Datumsbereichs.](../../assets/setup/aws-audience-sourcing/s3-schedule-refresh-frequency.png)

### Überprüfen und Abschließen der Verbindung {#review-and-complete}

Überprüfen Sie abschließend Ihre Konfigurationseinstellungen im Bildschirm Zusammenfassung . Diese Ansicht enthält eine Zusammenfassung der folgenden Abschnitte:

* **[!UICONTROL Datenverbindung]**: Zeigt die IAM-Rolle, den S3-Behälternamen und den von Ihnen konfigurierten Ordnerpfad an.
* **[!UICONTROL Details]**: Zeigt den Namen und die optionale Beschreibung Ihrer Datenverbindung an, damit Sie sie später identifizieren können.
* **[!UICONTROL Zuordnung]**: Listet auf, wie die Quellfelder aus Ihren hochgeladenen Zielgruppendateien (z. B. `HASHED_EMAIL`) den in Collaboration verwendeten Zielfeldern (z. B. Hash-E-Mails) zugeordnet werden.
* **[!UICONTROL Zeitplan]**: Fasst zusammen, wie oft die Verbindung Zielgruppendaten aktualisiert, und beschreibt den aktiven Datumsbereich für die Beschaffung.

Wählen Sie das Stiftsymbol aus, wenn Sie einen Abschnitt bearbeiten müssen. Klicken Sie **[!UICONTROL Fertig stellen]**, um alle Abschnitte zu bestätigen.

![Der Übersichtsbildschirm mit den Abschnitten Datenverbindung, Details, Zuordnung und Zeitplan.](../../assets/setup/aws-audience-sourcing/s3-connection-review-summary.png)

Es wird ein Bestätigungsdialogfeld angezeigt, in dem angegeben wird, dass die Datenverbindung erfolgreich erstellt wurde und dass die Zielgruppen-Beschaffung in Bearbeitung ist.

## Überprüfen der Quellzielgruppen {#review-sourced-audiences}

Nach Abschluss der Konfiguration beginnt Collaboration mit der Beschaffung von Zielgruppen aus Ihrem S3-Bucket. Audiences, die über einen [!DNL Amazon S3]-Bucket bezogen werden, werden auf der Registerkarte **[!UICONTROL Meine Audiences]** angezeigt und verfügen über dieselben Funktionen und Informationen wie Audiences, die aus Experience Platform bezogen werden.

Wenn die Zielgruppen-Beschaffung bereits läuft, wird oben auf dem Bildschirm ein Banner angezeigt. Einzelne Zielgruppen werden erst nach Abschluss der Beschaffung angezeigt.

![Die Registerkarte Zielgruppen , auf der angezeigt wird, dass für [!DNL Amazon S3] Zielgruppen gerade ein Sourcing durchgeführt wird.](../../assets/setup/aws-audience-sourcing/s3-audiences-sourcing-in-progress.png)

Sobald die S3-Zielgruppen bezogen wurden, wird Ihre Liste der verfügbaren Zielgruppen in einer tabellarischen oder Kartenansicht bereitgestellt.

>[!TIP]
>
>Die Zeit für die Zielgruppenbeschaffung hängt von der Größe Ihrer S3-Daten und der konfigurierten Aktualisierungshäufigkeit ab. Größere Datensätze oder weniger häufige Aktualisierungszeitpläne können länger dauern, bis sie im Arbeitsbereich &quot;**[!UICONTROL Zielgruppen“]** werden.

![Die Registerkarte Zielgruppen mit einer tabellarischen Liste von Zielgruppen aus der Quelle.](../../assets/setup/aws-audience-sourcing/s3-audiences-list-view.png)

Wählen Sie in der Rasteransicht oder Tabellenansicht ein Zeilenelement oder **[!UICONTROL Zielgruppe anzeigen]**, um eine Übersicht über eine bestimmte Zielgruppe zu erhalten. Darin werden der Status, die Quelle und der Name der Datenverbindung der Zielgruppe zusammen mit detaillierten Bedienfeldern für Folgendes angezeigt:

**[!UICONTROL Identitäten]**: Zeigt die Gesamtzahl der Identitäten und ihre Aufschlüsselung an, sobald Daten verfügbar sind.
**[!UICONTROL Kategorien]**: Listet alle Tags auf, die zum Organisieren oder Filtern der Zielgruppe verwendet werden.
**[!UICONTROL Verbindungszugriff]**: Gibt an, ob die Zielgruppe privat, öffentlich oder für bestimmte Mitarbeiter freigegeben ist.
**[!UICONTROL Metadaten-Sichtbarkeit]**: Definiert, welche Zielgruppeninformationen (z. B. Anzahl der Identitäten, Überschneidungsprozentsatz und Index) für Mitwirkende sichtbar sind.

Verwenden Sie diese Ansicht, um die Einstellungen für die Zielgruppenkonfiguration und Sichtbarkeit zu bestätigen, bevor Sie die Zielgruppe in Kooperationsprojekten verwenden.

Weitere Informationen finden [ in der ](https://experienceleague.adobe.com/en/docs/real-time-cdp-collaboration/using/setup/onboard-audiences#view-audiences-dashboard) zum Anzeigen von Zielgruppen-Dashboards .

## Anzeigen der S3-Datenverbindung {#view-s3-connection}

Die neu hinzugefügte [!DNL Amazon S3] ist sofort auf der Registerkarte **[!UICONTROL Meine Datenverbindungen]** verfügbar. Die Zielgruppenquelle wird als [!UICONTROL Amazon S3] angezeigt.

Ihre S3-Datenverbindung enthält dieselben Funktionen und Details wie andere Zielgruppendaten-Verbindungen, mit dem Unterschied, dass Sie Zielgruppen nicht direkt über diese Ansicht hinzufügen oder bearbeiten können.

>[!NOTE]
>
>[!DNL Amazon S3] Datenverbindungen können nicht bearbeitet werden. Einstellungen wie die Aktualisierungshäufigkeit können nach der Erstellung der Verbindung nicht mehr geändert werden. Um die Konfiguration zu aktualisieren, müssen Sie die vorhandene Verbindung löschen und eine neue erstellen.

![Die Registerkarte „Meine Datenverbindungen“, auf der die [!DNL Amazon S3] Datenverbindung mit Informationen zum Beschaffungsstatus angezeigt wird.](../../assets/setup/aws-audience-sourcing/s3-data-connections-tab.png)

## Nächste Schritte {#next-steps}

Sie haben jetzt Ihren [!DNL Amazon S3]-Speicher erfolgreich als Datenquelle in Collaboration konfiguriert und verbunden. Durch Abschluss dieses Workflows haben Sie die sichere Beschaffung von First-Party-Zielgruppendaten für die Aktivierung und Überschneidungsanalyse aktiviert.

Nach Abschluss des Einkaufs werden Ihre Zielgruppen im Arbeitsbereich **[!UICONTROL Meine Zielgruppen]** angezeigt, wo sie für die Zusammenarbeit und Aktivierung bereit sind. Detaillierte Informationen zu Verwaltungsoptionen finden Sie in der [Dokumentation „Quelle und Zielgruppen verwalten](./onboard-audiences.md).
