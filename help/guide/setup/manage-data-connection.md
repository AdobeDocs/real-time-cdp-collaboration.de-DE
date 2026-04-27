---
title: Datenverbindungen verwalten
description: Erfahren Sie, wie Sie in Real-Time CDP Collaboration Datenverbindungen verwalten, einschließlich Übereinstimmungsschlüsseln, Planung, Anwendungsfällen und Zielgruppenfilterung
audience: administrator, data engineer
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
TQID: https://experienceleague.adobe.com/QvkEpR1fJMZ5BXrucAzEtxFNSfSMS-2hIZvMSg63ySE
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1179
ht-degree: 5%

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
>abstract="Zeigen Sie die Zeitplandetails für Ihre Datenverbindung an und bearbeiten Sie bei Bedarf die Konfigurationen."

Zeigen Sie die Zeitplaneinstellungen für Ihre Datenverbindungen an und verwalten Sie sie. Die Planung bestimmt, wie oft die Zielgruppe aktualisiert wird.

Nachdem eine Datenverbindung erstellt wurde, können Sie ihre Aktualisierungshäufigkeit, ihr Start- und Enddatum direkt im Abschnitt **[!UICONTROL Planung]** des Arbeitsbereichs Datenverbindung aktualisieren.

>[!NOTE]
>
>Beim Bezug von Zielgruppen aus Adobe Experience Platform werden Zielgruppen innerhalb von 24 Stunden nach Herstellung der Datenverbindung verfügbar. Nach der ersten Beschaffung werden die Zielgruppendaten entsprechend der definierten Häufigkeit aktualisiert.

Weitere Informationen zur Planung finden Sie [&#x200B; Abschnitt „Planung](/help/guide/setup/onboard-audiences.md#schedule) im Handbuch zum Konfigurieren von Zielgruppen.

![Der Arbeitsbereich einer Datenverbindung mit hervorgehobenem Abschnitt „Planung“.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## Datenverbindung bearbeiten {#edit-data-connection}

Lesen Sie die folgenden Abschnitte, um zu erfahren, wie Sie die Übereinstimmungsschlüssel und Zeitplaneinstellungen einer vorhandenen Datenverbindung aktualisieren.

### Übereinstimmungsschlüssel bearbeiten {#edit-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_edit_measurement_data_connection_enrichment"
>title="Anreicherung"
>abstract="Das Deaktivieren der Anreicherung wird nicht unterstützt. Stattdessen können Sie die Join-Schlüssel der Anreicherung ändern."
>additional-url="https://www.adobe.com/go/rtcdp-collaboration-manage-dataconnections" text="Anreicherung"

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

![The dropdown menu displaying all available target fields to map with the new source field.](/help/assets/setup/manage-data-connection/select-target-field.png){zoomable="yes"}

After you finish mapping fields, review your updates and select **[!UICONTROL Confirm]** to apply the changes.

![The Match keys dialog showing the updated field mapping with the Confirm option highlighted.](/help/assets/setup/manage-data-connection/review-and-confirm.png){zoomable="yes"}

A confirmation dialog confirms that the match keys were updated successfully.

### Edit scheduling {#edit-scheduling}

Nachdem eine Datenverbindung erstellt wurde, können Sie ihre Aktualisierungshäufigkeit, ihr Start- und Enddatum direkt im Abschnitt **[!UICONTROL Planung]** des Arbeitsbereichs Datenverbindung aktualisieren.

You can edit the frequency of an existing data connection to better control how often audiences are refreshed. To edit the schedule, select **[!UICONTROL Edit]** from within the data connection in the scheduling card.

![The Scheduling section with the Edit option highlighted.](/help/assets/setup/manage-data-connection/edit-scheduling.png){zoomable="yes"}

A confirmation dialog appears, explaining that any changes to the data connection will apply to all associated audiences. Select **[!UICONTROL OK]** to confirm. You can choose to skip this confirmation in the future.

![Confirmation dialog showing that any changes to the data connection will apply to all associated audiences.](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

In the **[!UICONTROL Scheduling]** dialog, select the dropdown menu to update the **[!UICONTROL Frequency]**. Set the refresh frequency to run daily or every two to six days.

![The Scheduling dialog with the Frequency dropdown expanded to display audience refresh frequency options.](../../assets/setup/manage-data-connection/edit-frequency.png){zoomable="yes"}

Next, select **[!UICONTROL Date range]** if you want to update the period during which audiences are populated and refreshed.

![The Scheduling dialog showing the Date range dropdown expanded to edit the start and end dates for audience population and refresh.](../../assets/setup/manage-data-connection/edit-date-range.png){zoomable="yes"}

When you&#39;re done, review the updates and select **[!UICONTROL Save]** to apply your changes.

![The Scheduling dialog highlighting the updates and Save option.](../../assets/setup/manage-data-connection/scheduling-dialog.png){zoomable="yes"}

## Datenverbindung löschen

Deleting a data connection will remove all underlying audiences, associated settings, and usage across Collaboration. Diese Aktion kann nicht rückgängig gemacht werden.

To delete an existing data connection, select the delete icon (![Delete icon](/help/assets/common/delete.svg)) within an individual data connection&#39;s workspace.

![A data connections workspace with the delete option highlighted.](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

A confirmation dialogue will appear. Select **[!UICONTROL Delete]** to finish deleting the data connection.

![Das Dialogfeld „Datenverbindung löschen“ mit hervorgehobener Option „Löschen“.](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## Verwalten von Zielgruppen {#manage-audiences}

Unten im Arbeitsbereich wird eine Liste von Audiences angezeigt, die mit der Datenverbindung verbunden sind. Die Liste zeigt einen kurzen Überblick über jede Zielgruppe, einschließlich ihres Status, ihrer Quelle und ihres Verbindungszugriffs. Um die Kategorien, den Verbindungszugriff oder die Sichtbarkeit der Metadaten einer Zielgruppe zu bearbeiten, wählen Sie den Namen der Zielgruppe aus. Eine vollständige Anleitung zum Verwalten einer Zielgruppe finden Sie im [Anzeigen einzelner Zielgruppen](./onboard-audiences.md#view-individual-audiences).

![Ein Arbeitsbereich für Datenverbindungen mit hervorgehobenen Zielgruppen.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## Nächste Schritte

Nach der Verwaltung Ihrer Datenverbindungen können Sie [Überschneidungen](/help/guide/collaborate/discover.md) zwischen Ihren Zielgruppen und den Zielgruppen entdecken, die Ihr Mitarbeiter entdeckt hat.
