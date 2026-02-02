---
title: CSV-Datei für Zielgruppen-Sourcing hochladen
description: Erfahren Sie, wie Sie Ihre CSV-Datei als Self-Service-Datenquelle hochladen, um Zielgruppendaten in Real-Time CDP Collaboration aufzunehmen.
source-git-commit: 96d3f87cedcfde73ce01c2b53c0b2ce4365fd277
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 0%

---

# CSV-Datei für Zielgruppen-Sourcing hochladen

In diesem Handbuch werden Schritte zum Hochladen einer CSV-Datei in die Adobe Real-Time CDP Collaboration-Benutzeroberfläche beschrieben, um Ihre Zielgruppendaten für die Verwendung in Kooperationsprojekten zu beziehen.

## Übersicht {#overview}

Der CSV-Datei-Upload ist eine Methode, um First-Party-Zielgruppendaten für Collaboration-Projekte zu beziehen. Dies ist eine Alternative zum [Verbinden Ihres AWS S3-Buckets](./configure-aws-s3-audience-sourcing.md) oder zum [&#x200B; von Zielgruppen aus Experience Platform](./onboard-audiences.md).

Folgen Sie diesem Workflow, um eine CSV-Datei mit Ihren Zielgruppendaten in Collaboration hochzuladen, um First-Party-Zielgruppen in der Quelle zu verwalten. Sie können Identitätsfelder für die Aktivierung und Überschneidungsanalyse zuordnen. Sobald Ihre Datei hochgeladen und verarbeitet wurde, wird die Zielgruppe aus der Quelle im Arbeitsbereich **[!UICONTROL Meine Zielgruppen]** verfügbar, wo Sie Ihre Collaboration-Projekte überprüfen, aktivieren und verwalten können.

>[!IMPORTANT]
>
>* Zielgruppen, die über den CSV-Upload bezogen werden, sind **7 Tage lang**. Nach Ablauf dieses Zeitraums muss die Zielgruppe erneut hochgeladen werden, um sie in Ihren Kooperationsprojekten verwenden zu können.
>
>* Zu diesem Zeitpunkt können Sie pro Sitzung eine CSV-Datei hochladen. Um weitere Audiences hinzuzufügen, schließen Sie den Upload-Workflow für jede Datei, die Sie beziehen möchten, erneut ab.

## Voraussetzungen {#prerequisites}

Bevor Sie CSV-Dateien für die Zielgruppen-Beschaffung hochladen können, stellen Sie sicher, dass Sie Folgendes haben:

* Das Onboarding eines Kontos in Real-Time CDP Collaboration wurde abgeschlossen. Eine [&#x200B; Anleitung finden Sie unter &#x200B;](./onboard-account.md) Ihres Kontos .
* Die erforderlichen Berechtigungen, um Zielgruppen in Ihrer Organisation hinzuzufügen.
* Eine CSV-Datei mit Ihren Zielgruppendaten mit Identitätsfeldern wie E-Mail oder Telefon.

## CSV-Datei hochladen {#upload-csv-file}

Wählen Sie im Arbeitsbereich **[!UICONTROL Setup]** **[!UICONTROL auf der Registerkarte „Meine Zielgruppen]** das Symbol zum Hinzufügen (![Hinzufügen) aus.](/help/assets/icons/plus.png)) und wählen Sie dann **[!UICONTROL Audience]** aus.

Wenn dies Ihre erste Zielgruppe ist, können Sie auch die Option **[!UICONTROL Hinzufügen]** auswählen.

![Die Registerkarte „Meine Zielgruppen“ im Arbeitsbereich „Setup“ mit dem Symbol „Hinzufügen“ und der Option „Zielgruppe hinzufügen“ wird angezeigt.](../../assets/setup/add-manage-audiences/add-audiences.png)

Der Workflow „Zielgruppe hinzufügen“ wird angezeigt. Wählen Sie **[!UICONTROL Neue Datenverbindung hinzufügen]** und dann **[!UICONTROL Weiter]** aus.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit hervorgehobener Option „Neue Datenverbindung hinzufügen“.](../../assets/setup/add-manage-audiences/add-data-connection.png){zoomable="yes"}

### CSV-Datei als Datenverbindung auswählen {#select-csv-file}

Wählen **[!UICONTROL CSV-]**) als Datenverbindung aus, gefolgt von **[!UICONTROL Weiter]**.

![Der Bildschirm zur Auswahl der Datenverbindung mit CSV-Datei ist als auswählbare Option verfügbar.](../../assets/setup/csv-audience-sourcing/select-csv-data-connection.png)

### Datei auswählen {#select-file}

Wählen Sie **[!UICONTROL Vom Computer auswählen]**, um eine CSV-Datei von Ihrem lokalen System hochzuladen. Alternativ können Sie die CSV-Datei, die Sie hochladen möchten, per Drag-and-Drop in das Bedienfeld [!UICONTROL CSV-Datei per Drag-and-Drop &#x200B;]&quot; ziehen.

>[!IMPORTANT]
>
>Es werden nur CSV-Dateien unterstützt. Die maximale Dateigröße beträgt **GB**.

![Wählen Sie eine CSV-Datei aus, die Zielgruppendaten aus Ihrem lokalen System enthält.](../../assets/setup/csv-audience-sourcing/select-file.png)

Nach dem Hochladen zeigt die Benutzeroberfläche eine Zusammenfassung an, die die Anzahl der Spalten, eine geschätzte Zeilenanzahl, die Struktur der Datei und eine Vorschau der ersten 10 Datenzeilen enthält.

Überprüfen Sie die Zusammenfassung und klicken Sie dann auf **[!UICONTROL Weiter]**.

![Vorschau der Beispieldaten der Audience aus Ihrer CSV-Datei.](../../assets/setup/csv-audience-sourcing/preview-sample-data.png)

#### Datei ersetzen {#replace-file}

Wenn Sie eine andere CSV-Datei hochladen müssen, wählen Sie **[!UICONTROL Datei ersetzen]** und wählen Sie Ihre neue Datei aus. Die Benutzeroberfläche wird dann aktualisiert, um eine aktualisierte Zusammenfassung der neuen Daten anzuzeigen.

Klicken Sie nach der Überprüfung der überarbeiteten Zusammenfassung auf **[!UICONTROL Weiter]**.

![Wählen Sie die Option Datei ersetzen aus, um eine andere CSV-Datei hochzuladen.](../../assets/setup/csv-audience-sourcing/replace-file.png)

### Einverständnisbestätigung bestätigen {#confirm-consent}

Bevor Sie fortfahren, müssen Sie bestätigen, dass aus Ihren Zielgruppendaten Einverständnis-Opt-outs entfernt wurden. Collaboration erfordert saubere Zielgruppendaten ohne Benutzer, die sich gegen die Datenfreigabe entschieden haben.

Markieren Sie zur Bestätigung das Bestätigungsfeld **[!UICONTROL OK]**. Das Dialogfeld wird geschlossen und Sie gelangen zum Bildschirm Felder zuordnen .

![Das Dialogfeld zur Bestätigung des Einverständnis-Opt-outs, das vor dem Fortfahren bestätigt werden muss.](../../assets/setup/csv-audience-sourcing/consent-optout-acknowledgment.png)

### Quellidentitätsfelder zuordnen {#map-fields}

Die Feldzuordnung bestimmt, wie Collaboration Ihre Zielgruppendaten für die Aktivierung und Überschneidungsanalyse verwendet. Verwenden **[!UICONTROL auf dem Bildschirm]** Zuordnungsfelder“ die Dropdown-Menüs, um jedes Quellidentitätsfeld aus Ihrer CSV-Datei dem entsprechenden Zielfeld in Collaboration zuzuordnen.

Wenn Sie zusätzliche Details zu einem Zielfeld benötigen, einschließlich des Datentyps oder der Beschreibung, wählen Sie **[!UICONTROL Zielfelddetails]** aus, um weitere Informationen zu erhalten.

![Das Dropdown-Menü zum Zuordnen eines Quellidentitätsfelds aus Ihren CSV-Zielgruppendaten zum Zielfeld in Collaboration.](../../assets/setup/csv-audience-sourcing/map-fields.png)

Überprüfen Sie als Nächstes die zugeordneten Felder und wählen Sie dann **[!UICONTROL Weiter]** aus.

![Der Bildschirm für die Feldzuordnung mit den zugeordneten Quell- und Ziel-Identitätsfeldern.](../../assets/setup/csv-audience-sourcing/confirm-mapped-fields.png)

### Überprüfen und Abschließen des Uploads {#review-and-complete}

Der Bildschirm **[!UICONTROL Überprüfen]** wird mit einer Zusammenfassung der Zielgruppeneinstellungen aus Ihrer CSV-Datei angezeigt. Überprüfen Sie die Informationen in den folgenden Abschnitten:

* **[!UICONTROL Dateiinformationen]**: Zeigt den Dateinamen, die Anzahl der Spalten und die geschätzte Zeilenanzahl an.
* **[!UICONTROL Zuordnung]**: Listet auf, wie die Quellfelder aus Ihrer hochgeladenen Zielgruppendatei (z. B. `email`) den in Collaboration verwendeten Zielfeldern (z. B. Hash-E-Mails) zugeordnet werden.

Wählen Sie das Stiftsymbol aus, wenn Sie einen Abschnitt bearbeiten müssen. Klicken Sie **[!UICONTROL Fertig stellen]**, um alle Abschnitte zu bestätigen.

![Überprüfen Sie die Zusammenfassung der Upload-Einstellungen einschließlich CSV-Dateiinformationen und Details zur Feldzuordnung.](../../assets/setup/csv-audience-sourcing/review-upload-summary.png)

Unterhalb der Zusammenfassungsabschnitte wird eine Fortschrittsleiste angezeigt, die den Upload-Fortschritt anzeigt. Nach Abschluss des Uploads wird in einem Bestätigungsdialogfeld bestätigt, dass Ihre CSV-Zielgruppe erstellt wurde und die Zielgruppen-Beschaffung in Bearbeitung ist.

![Nach dem Hochladen der Datei wird ein Bestätigungsdialogfeld angezeigt, in dem angegeben wird, dass eine CSV-Zielgruppe erstellt wurde und die Zielgruppen-Beschaffung in Bearbeitung ist.](../../assets/setup/csv-audience-sourcing/upload-success-sourcing-in-progress.png)

## Überprüfen der Quellzielgruppen {#review-sourced-audiences}

Nach dem Hochladen der CSV-Datei beginnt Collaboration mit dem Bezug von Zielgruppen aus der Datei. Dieser Vorgang kann mehrere Minuten dauern. Nach Abschluss der Beschaffung stehen Ihre Zielgruppen auf der Registerkarte **[!UICONTROL Meine Zielgruppen]** mit denselben Funktionen und Informationen wie Zielgruppen aus Experience Platform zur Verfügung.

![Die Registerkarte Zielgruppen , auf der in der Rasteransicht eine Liste der Zielgruppen aus der Quelle angezeigt wird.](../../assets/setup/csv-audience-sourcing/csv-audiences-list.png)

Wählen Sie in der Rasteransicht oder Tabellenansicht ein Zeilenelement oder **[!UICONTROL Zielgruppe anzeigen]**, um eine Übersicht über eine bestimmte Zielgruppe zu erhalten. Darin werden der Status, die Quelle und der Name der Datenverbindung der Zielgruppe zusammen mit detaillierten Bedienfeldern für Folgendes angezeigt:

**[!UICONTROL Identitäten]**: Zeigt die Gesamtzahl der Identitäten und ihre Aufschlüsselung an, sobald Daten verfügbar sind.
**[!UICONTROL Kategorien]**: Zeigt alle Tags an, die zum Organisieren oder Filtern der Zielgruppe verwendet werden.
**[!UICONTROL Verbindungszugriff]**: Zeigt an, ob die Zielgruppe privat, öffentlich oder für bestimmte Mitarbeiter freigegeben ist.
**[!UICONTROL Metadaten-Sichtbarkeit]**: Zeigt an, welche Zielgruppeninformationen (wie Identitätsanzahl, Überschneidungsprozentsatz und Index) für Mitwirkende sichtbar sind.

Verwenden Sie diese Ansicht, um die Einstellungen für die Zielgruppenkonfiguration und Sichtbarkeit zu bestätigen, bevor Sie die Zielgruppe in Kooperationsprojekten verwenden. Weitere Informationen finden Sie unter [Anzeigen einer einzelnen Zielgruppe](./onboard-audiences.md#view-individual-audiences).

## Nächste Schritte {#next-steps}

Sie haben jetzt Ihre CSV-Datei erfolgreich in Collaboration hochgeladen. Nach Abschluss der Beschaffung haben Sie folgende Möglichkeiten:

* Erstellen Sie Kooperationsprojekte mit Ihren Zielgruppen aus der Quelle. Siehe [Zielgruppen entdecken](../../guide/collaborate/discover.md).
* Aktivieren Sie Zielgruppen für verbundene Ziele. Siehe [Aktivieren von Zielgruppen](../../guide/collaborate/activate.md).
* Überprüfen Sie Zielgruppenüberschneidungen und Einblicke. Siehe [Messen der Kampagnenleistung](../../guide/collaborate/measure.md).
* Verwalten Sie Ihre Zielgruppeneinstellungen und Sichtbarkeit. Siehe [Source und Zielgruppen verwalten](./onboard-audiences.md).

Weitere Informationen zu anderen Zielgruppen-Beschaffungsmethoden finden Sie unter [Konfigurieren von AWS S3 für Zielgruppen-Beschaffung](./configure-aws-s3-audience-sourcing.md) oder [Source-Zielgruppen aus Experience Platform](./onboard-audiences.md).
