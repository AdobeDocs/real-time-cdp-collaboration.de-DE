---
title: Datenverbindungen verwalten
description: Erfahren Sie, wie Sie in Real-Time CDP Collaboration Datenverbindungen verwalten, einschließlich Übereinstimmungsschlüsseln, Planung, Anwendungsfällen und Zielgruppenfilterung
audience: administrator, data engineer
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
TQID: https://experienceleague.adobe.com/QvkEpR1fJMZ5BXrucAzEtxFNSfSMS-2hIZvMSg63ySE
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 867dad8a34086c3dd9a36f35577de7889c28a727
workflow-type: tm+mt
source-wordcount: 1253
ht-degree: 7%

---

# Datenverbindungen verwalten

{{limited-availability-release-note}}

## Überblick

Verwenden Sie Datenverbindungen in Real-Time CDP Collaboration, um Zielgruppen von verschiedenen Plattformen aus zu beziehen. Erfahren Sie, wie Sie Übereinstimmungsschlüssel verwalten und die Aktualisierung von Daten für Ihre vorhandenen Datenverbindungen planen. Darüber hinaus können Sie Zielgruppen nach verschiedenen Attributen filtern, um detailliertere Einblicke zu erhalten.

>[!NOTE]
>
>Informationen zum Erstellen einer neuen Datenverbindung finden Sie unter [Hinzufügen und Verwalten von Zielgruppen](./onboard-audiences.md).

## Datenverbindungen anzeigen

Um vorhandene Datenverbindungen anzuzeigen, navigieren Sie zu **[!UICONTROL Setup]** und wählen Sie dann die Registerkarte **[!UICONTROL Meine Datenverbindungen]** aus. Es werden alle Ihre aktuellen Verbindungsdaten angezeigt, die jeweils eine kurze Übersicht enthalten. Um eine vollständige Ansicht der Informationen einer Datenverbindung zu erhalten, einschließlich der Übereinstimmungsschlüssel, Zeitplandetails und Zielgruppen, wählen Sie **[!UICONTROL Datenverbindung anzeigen]** für die entsprechende Verbindung aus.

![Arbeitsbereich einrichten, auf dem die Registerkarte „Meine Datenverbindungen“ angezeigt und hervorgehoben wird.](/help/assets/setup/manage-data-connection/my-data-connections.png){zoomable="yes"}

### Übereinstimmungsschlüssel {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="Übereinstimmungsschlüssel"
>abstract="Übereinstimmungsschlüssel bestimmen, wie Daten aus verschiedenen Quellen zugeordnet werden. Die unten angezeigten Übereinstimmungsschlüssel sind die Zielfelder, denen Sie Ihre Quellfelder zugeordnet haben."

Übereinstimmungsschlüssel sind die Zielfelder, denen Sie [Ihre Quellfelder zugeordnet haben](./onboard-audiences.md#map-fields). Weitere Informationen zur Funktionsweise von Übereinstimmungsschlüsseln finden Sie im Handbuch [Übereinstimmungsschlüssel](./onboard-account.md#set-up-match-keys) .

![Ein Arbeitsbereich für Datenverbindungen mit hervorgehobenem Abschnitt „Übereinstimmungsschlüssel“.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### Planung {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="Planung"
>abstract="Zeigen Sie die Zeitplanungsdetails für Ihre Datenverbindung an und bearbeiten Sie die Konfigurationen bei Bedarf."

Zeigen Sie die Zeitplaneinstellungen für Ihre Datenverbindungen an und verwalten Sie sie. Die Planung bestimmt, wie oft die Zielgruppe aktualisiert wird.

Nachdem eine Datenverbindung erstellt wurde, können Sie ihre Aktualisierungshäufigkeit, ihr Start- und Enddatum direkt im Abschnitt **[!UICONTROL Planung]** des Arbeitsbereichs Datenverbindung aktualisieren.

>[!NOTE]
>
>Beim Bezug von Zielgruppen aus Adobe Experience Platform werden Zielgruppen innerhalb von 24 Stunden nach Herstellung der Datenverbindung verfügbar. Nach der ersten Beschaffung werden die Zielgruppendaten entsprechend der definierten Häufigkeit aktualisiert.

Weitere Informationen zur Planung finden Sie [ Abschnitt „Planung](/help/guide/setup/onboard-audiences.md#schedule) im Handbuch zum Konfigurieren von Zielgruppen.

![Der Arbeitsbereich einer Datenverbindung mit hervorgehobenem Abschnitt „Planung“.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## Datenverbindung bearbeiten {#edit-data-connection}

Lesen Sie die folgenden Abschnitte, um zu erfahren, wie Sie die Übereinstimmungsschlüssel und Zeitplaneinstellungen einer vorhandenen Datenverbindung aktualisieren.

### Übereinstimmungsschlüssel bearbeiten {#edit-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_edit_measurement_data_connection_enrichment"
>title="Anreicherung"
>abstract="Das Deaktivieren der Anreicherung wird nicht unterstützt. Stattdessen können Sie die Join-Schlüssel der Anreicherung ändern."
>additional-url="https://www.adobe.com/go/rtcdp-collaboration-manage-dataconnections_de" text="Anreicherung"

>[!IMPORTANT]
>
>Beachten Sie Folgendes, bevor Sie die Übereinstimmungsschlüssel für eine Datenverbindung bearbeiten:
>
>* Für Datenverbindungen können nur Übereinstimmungsschlüssel verwendet werden, die für Ihr Konto konfiguriert sind.
>* Derzeit können Sie zusätzliche Übereinstimmungsschlüssel zu einer Datenverbindung hinzufügen, aber sobald ein Übereinstimmungsschlüssel aktiviert ist, kann er nicht mehr entfernt werden.

Wählen **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Übereinstimmungsschlüssel]** aus.

![Der Abschnitt „Übereinstimmungsschlüssel“ mit hervorgehobener Option „Bearbeiten“.](/help/assets/setup/manage-data-connection/edit-match-keys.png){zoomable="yes"}

Es wird ein Bestätigungsdialogfeld angezeigt, in dem erklärt wird, dass alle Änderungen an der Datenverbindung für alle verknüpften Zielgruppen gelten. Klicken **[!UICONTROL zur]** auf OK. Sie können diese Bestätigung später überspringen.

![Bestätigungsdialogfeld, das anzeigt, dass alle Änderungen an der Datenverbindung für alle verknüpften Zielgruppen gelten.](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

Im Dialogfeld **[!UICONTROL Übereinstimmungsschlüssel]** können Sie die vorhandenen Zuordnungen zwischen Quellfeldern und den entsprechenden Zielfeldern (Übereinstimmungsschlüssel) anzeigen. Sie können einen Übereinstimmungsschlüssel bearbeiten, indem Sie das zugeordnete Quellfeld aktualisieren, oder zusätzliche Zuordnungsfeldzeilen hinzufügen, um neue Übereinstimmungsschlüssel auszufüllen.

![Das Dialogfeld Schlüssel abgleichen , das die vorhandenen Zuordnungen zwischen Quellfeldern und den entsprechenden Zielfeldern anzeigt.](/help/assets/setup/manage-data-connection/match-keys-dialog.png){zoomable="yes"}

#### Übereinstimmungsschlüssel hinzufügen {#add-match-keys}

Wählen Sie **[!UICONTROL Feld hinzufügen]** aus, um eine neue Feldzeile hinzuzufügen.

![Nach Auswahl von Feld hinzufügen zeigt das Dialogfeld Übereinstimmungsschlüssel ein leeres neues Zuordnungsfeld an, das bereit zur Eingabe ist.](/help/assets/setup/manage-data-connection/add-new-field.png){zoomable="yes"}

Wählen Sie anschließend das leere Quellfeld aus. Das Dialogfeld **[!UICONTROL Quellfeld auswählen]** wird mit den Optionen **[!UICONTROL Identity-]** und **[!UICONTROL Profilattribute]** angezeigt. Sie können die Liste filtern und das gewünschte Quellfeld mit der Suchoption finden.

Wählen Sie das gewünschte Quellfeld und dann **[!UICONTROL Auswählen]** aus.

![Das Dialogfeld „Quellfeld auswählen“ mit ausgewählter GAID-Option.](/help/assets/setup/manage-data-connection/select-source-field.png){zoomable="yes"}

Verwenden **[!UICONTROL im Dialogfeld]**&#x200B;Übereinstimmungsschlüssel“ das Dropdown-Menü, um das neue Quellfeld einem Zielfeld zuzuordnen. Alle verfügbaren Zielfelder sind die für Ihr Mitarbeiter-Konto konfigurierten Übereinstimmungsschlüssel. Wenn das gewünschte Zielfeld nicht angezeigt wird, fügen Sie [die Übereinstimmungsschlüssel Ihres Kontos bearbeiten](./onboard-account.md#edit-match-keys) hinzu.

Verwenden Sie die Option **[!UICONTROL Umwandlung anwenden]**, wenn Sie ein nicht gehashtes Feld in ein gehashtes Zielfeld eingeben möchten, z. B. wenn Sie dem Zielfeld **[!UICONTROL gehashte E-Mail]** ein reines Text-E-Mail-Quellfeld zuordnen.

![Das Dropdown-Menü mit allen verfügbaren Zielfeldern, die dem neuen Quellfeld zugeordnet werden sollen.](/help/assets/setup/manage-data-connection/select-target-field.png){zoomable="yes"}

##### [!DNL Demdex ID (ECID)] hinzufügen {#add-demdex-id-ecid}

Wenn Sie [!DNL Demdex ID (ECID)] als Übereinstimmungsschlüssel hinzufügen möchten, stellen Sie zunächst sicher, dass er in [ Kontoeinstellungen aktiviert ](../setup/onboard-account.md#set-up-match-keys). Weitere Informationen zum [!DNL Demdex ID (ECID)] finden Sie unter [Unterstützte Übereinstimmungsschlüssel](../setup/onboard-account.md#supported-match-keys).

Fügen Sie im **[!UICONTROL Übereinstimmungsschlüssel]** eine neue Zeile für das Zuordnungsfeld hinzu. Wählen Sie dann **[!UICONTROL ECID]** als Quellfeld und **[!UICONTROL Demdex-ID (ECID)]** als Zielfeld aus der Dropdown-Liste aus.

![Das Dialogfeld „Übereinstimmungsschlüssel“ mit hervorgehobenem Zuordnungsfeld für den Übereinstimmungsschlüssel der Demdex-ID (ECID).](/help/assets/setup/manage-data-connection/demdex-id-ecid-match-key.png){zoomable="yes"}

Nachdem Sie die Zuordnungsfelder abgeschlossen haben, überprüfen Sie Ihre Aktualisierungen und wählen Sie **[!UICONTROL Bestätigen]**, um die Änderungen anzuwenden.

![Das Dialogfeld „Übereinstimmungsschlüssel“, das die aktualisierte Feldzuordnung mit hervorgehobener Option „Bestätigen“ anzeigt.](/help/assets/setup/manage-data-connection/review-and-confirm.png){zoomable="yes"}

Ein Bestätigungsdialogfeld bestätigt, dass die Übereinstimmungsschlüssel erfolgreich aktualisiert wurden.

### Zeitplan bearbeiten {#edit-scheduling}

Nachdem eine Datenverbindung erstellt wurde, können Sie ihre Aktualisierungshäufigkeit, ihr Start- und Enddatum direkt im Abschnitt **[!UICONTROL Planung]** des Arbeitsbereichs Datenverbindung aktualisieren.

Sie können die Häufigkeit einer vorhandenen Datenverbindung bearbeiten, um besser steuern zu können, wie oft Zielgruppen aktualisiert werden. Um den Zeitplan zu bearbeiten, wählen Sie **[!UICONTROL Bearbeiten]** in der Datenverbindung auf der Planungskarte aus.

![Der Planungsabschnitt mit der hervorgehobenen Option „Bearbeiten“.](/help/assets/setup/manage-data-connection/edit-scheduling.png){zoomable="yes"}

Es wird ein Bestätigungsdialogfeld angezeigt, in dem erklärt wird, dass alle Änderungen an der Datenverbindung für alle verknüpften Zielgruppen gelten. Klicken **[!UICONTROL zur]** auf OK. Sie können diese Bestätigung später überspringen.

![Bestätigungsdialogfeld, das anzeigt, dass alle Änderungen an der Datenverbindung für alle verknüpften Zielgruppen gelten.](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

Wählen Sie **[!UICONTROL Dialogfeld &quot;]**&quot; das Dropdown-Menü aus, um die **[!UICONTROL Häufigkeit]** zu aktualisieren. Stellen Sie die Aktualisierungshäufigkeit so ein, dass sie täglich oder alle zwei bis sechs Tage ausgeführt wird.

![Das Dialogfeld Planung mit dem Dropdown-Menü Häufigkeit wurde erweitert, um die Optionen für die Aktualisierungshäufigkeit der Zielgruppe anzuzeigen.](../../assets/setup/manage-data-connection/edit-frequency.png){zoomable="yes"}

Wählen Sie als Nächstes **[!UICONTROL Datumsbereich]** aus, wenn Sie den Zeitraum aktualisieren möchten, in dem Zielgruppen aufgefüllt und aktualisiert werden.

![Das Dialogfeld Planung mit dem Dropdown-Menü Datumsbereich wurde erweitert, um das Start- und Enddatum für die Zielgruppenpopulation zu bearbeiten und zu aktualisieren.](../../assets/setup/manage-data-connection/edit-date-range.png){zoomable="yes"}

Wenn Sie fertig sind, überprüfen Sie die Aktualisierungen und wählen Sie **[!UICONTROL Speichern]** aus, um Ihre Änderungen anzuwenden.

![Das Dialogfeld „Planung“ mit hervorgehobenen Optionen „Aktualisierungen und Speichern“.](../../assets/setup/manage-data-connection/scheduling-dialog.png){zoomable="yes"}

## Datenverbindung löschen {#delete-data-connection}

Durch das Löschen einer Datenverbindung werden alle zugrunde liegenden Zielgruppen, zugehörigen Einstellungen und die Verwendung in Collaboration entfernt. Diese Aktion kann nicht rückgängig gemacht werden.

Um eine vorhandene Datenverbindung zu löschen, wählen Sie das Löschsymbol (![Löschsymbol) ](/help/assets/common/delete.svg) Arbeitsbereich einer einzelnen Datenverbindung aus.

![Ein Arbeitsbereich für Datenverbindungen mit hervorgehobener Löschoption.](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

Ein Bestätigungsdialogfeld wird angezeigt. Wählen Sie **[!UICONTROL Löschen]** aus, um das Löschen der Datenverbindung abzuschließen.

![Das Dialogfeld „Datenverbindung löschen“ mit hervorgehobener Option „Löschen“.](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## Verwalten von Zielgruppen {#manage-audiences}

Unten im Arbeitsbereich wird eine Liste von Audiences angezeigt, die mit der Datenverbindung verbunden sind. Die Liste zeigt einen kurzen Überblick über jede Zielgruppe, einschließlich ihres Status, ihrer Quelle und ihres Verbindungszugriffs. Um die Kategorien, den Verbindungszugriff oder die Sichtbarkeit der Metadaten einer Zielgruppe zu bearbeiten, wählen Sie den Namen der Zielgruppe aus. Eine vollständige Anleitung zum Verwalten einer Zielgruppe finden Sie im [Anzeigen einzelner Zielgruppen](./onboard-audiences.md#view-individual-audiences).

![Ein Arbeitsbereich für Datenverbindungen mit hervorgehobenen Zielgruppen.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## Nächste Schritte

Nach der Verwaltung Ihrer Datenverbindungen können Sie [Überschneidungen](/help/guide/collaborate/discover.md) zwischen Ihren Zielgruppen und den Zielgruppen entdecken, die Ihr Mitarbeiter entdeckt hat.
