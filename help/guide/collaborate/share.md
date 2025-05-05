---
title: Zielgruppen freigeben
description: Erfahren Sie, wie Sie Audiences für Werbekampagnen mit Ihren Mitwirkenden teilen können.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0fdf0598-89c9-452d-a2e3-ce868df0b9d2
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 6%

---

# Zielgruppen freigeben

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>Der **[!UICONTROL Freigabe]**-Arbeitsbereich ist nur verfügbar, wenn der Anwendungsfall **Zielgruppenfreigabe und -aktivierung** während [ Verbindungsprozesses aktiviert ](../connect/establishing-connections.md#connection-settings). Weitere Informationen zu Anwendungsfällen finden Sie im Handbuch [Verwalten von ](./manage-projects.md#project-use-cases)&quot;.

Erfahren Sie, wie Sie als Advertiser Zielgruppen mit Ihren Publishern teilen können, damit diese Kampagnen ausführen können. Wenn Ihre Zusammenarbeit den Anwendungsfall **Zielgruppen entdecken** aktiviert hat, führen Sie zunächst Überschneidungsberichte auf der Registerkarte [Entdecken](/help/guide/collaborate/discover.md) aus, um die besten Zielgruppen für die Freigabe zu ermitteln.

## Freigeben neuer Zielgruppen

Um mit der Freigabe von Audiences zu beginnen, navigieren Sie **[!UICONTROL Registerkarte]** Freigeben“ in Ihrem Projektarbeitsbereich. Nur **Advertiser-Organisationen** können Zielgruppen für Kampagnen freigeben. Auf dieser Registerkarte können Sie freigegebene Audiences überprüfen und verwalten.

Wählen Sie das **Plus-Symbol (+)** oder die Option **[!UICONTROL Zielgruppe freigeben]** aus, wenn keine vorherigen Zielgruppen freigegeben wurden, um den Prozess der Zielgruppenfreigabe zu starten.

![Standardansicht ohne freigegebene Zielgruppen.](/help/assets/collaborate/share/share-new-audiences.png)

Es wird ein neues Bedienfeld angezeigt, in dem Sie die Zielgruppen auswählen können, die Sie für Ihren Mitarbeiter freigeben möchten.

![Workflow zum Freigeben neuer Zielgruppen.](/help/assets/collaborate/share/share-audiences-workflow.png)

### Zielgruppen zur Freigabe auswählen

Im Fenster zur Zielgruppenauswahl können Sie nach bestimmten Zielgruppen suchen, die Sie freigeben möchten, indem Sie den Namen der Zielgruppe in die Suchleiste eingeben. Wählen Sie **[!UICONTROL Zielgruppen durchsuchen]** und verwenden Sie die verfügbaren Sortieroptionen, um die gewünschten Zielgruppen zu finden.

![Ansicht „Zielgruppen durchsuchen“ mit ausgewählten Zielgruppen.](/help/assets/collaborate/share/browse-audiences-view.png)

### Bearbeiten von Übereinstimmungsschlüsseln und Festlegen von Zielgruppenoptionen

Nach Auswahl der gewünschten Zielgruppen, die freigegeben werden sollen, können Sie jetzt andere Konfigurationsoptionen für die Freigabeaktivität auswählen.

![Übereinstimmungsschlüssel bearbeiten und Auswahl für Ziel oder Unterdrückung hervorgehoben](/help/assets/collaborate/share/match-keys-and-targeting.png)

Wählen Sie **[!UICONTROL Übereinstimmungsschlüssel bearbeiten]**, um anzugeben, welche Übereinstimmungsschlüssel für die Identitäten in der Zielgruppe verwendet werden sollen. Diese Optionen werden von den Einstellungen übernommen, die beim erstmaligen Einrichten der Verbindung zwischen Partnern ausgewählt wurden. Sie können die zu diesem Zeitpunkt ausgewählten Übereinstimmungsschlüssel entfernen, wenn sie nicht für diese spezifische Kampagne gelten. Sie können jedoch zu diesem Zeitpunkt keine neuen Übereinstimmungsschlüssel hinzufügen.

![Übereinstimmungsschlüssel bearbeiten.](/help/assets/collaborate/share/update-match-keys.png)

Wählen Sie für jede Zielgruppe aus, ob die Mitglieder dieser Zielgruppe in der Kampagne angesprochen oder unterdrückt werden sollen. Unterdrückte Profile sind ausdrücklich nicht Teil der vom Publisher aktivierten Zielgruppe.

### Festlegen der Häufigkeit und des Intervalls für die Zielgruppenaktualisierung

Legen Sie abschließend die gewünschte Häufigkeit und den gewünschten Datumsbereich für die Zielgruppenaktualisierung fest. Die derzeit unterstützten Modi für die Aktualisierung der Zielgruppe sind **[!UICONTROL Einmal]** und **[!UICONTROL Täglich]**.

Bei Auswahl **[!UICONTROL Einmal]** wird die Zielgruppenzugehörigkeit nicht über die gesamte Dauer einer Kampagne aktualisiert. Bei Auswahl **[!UICONTROL Täglich]** wird die Zielgruppenzugehörigkeit während der gesamten Dauer einer Kampagne einmal täglich aktualisiert.

![Häufigkeitsoptionen hervorgehoben.](/help/assets/collaborate/share/audience-refresh-frequency.png)

Wenn Sie mit Ihrer Auswahl zufrieden sind, klicken Sie auf **[!UICONTROL Freigeben]**, um den Workflow abzuschließen.

>[!SUCCESS]
>
>Auf der Registerkarte **[!UICONTROL Freigabe“ wird jetzt eine neue Aktivität zur]** angezeigt. Falls gewünscht, können Sie zurück gehen und jede von Ihnen getroffene Auswahl bearbeiten.

## Anzeigen aktuell freigegebener Zielgruppen

Auf der Registerkarte **[!UICONTROL Freigabe]** können Sie die Zielgruppen anzeigen, die derzeit von den Mitwirkenden gemeinsam genutzt werden und in Aktivitäten zur Zielgruppenfreigabe gruppiert sind.

![Übersicht über die Registerkarte „Freigabe“.](/help/assets/collaborate/share/share-tab-overview.png)

<!--

The banner at the top of the page shows figures across all audience sharing activities. 

![The hero banner in the sharing tab.](/help/assets/collaborate/share/share-hero-banner.png)


|Metric | Description |
|---------|----------|
| **[!UICONTROL Shared audiences]** | Indicates the number of audiences shared between collaborators in this project, across all audience sharing modules. |
| **[!UICONTROL Estimated addressable reach]** | Indicates the approximate number of profiles that you can reach across all the audiences that are currently shared in the project. [TODO: ADD INFORMATION ABOUT HOW THIS IS CALCULATED] |
| **[!UICONTROL Target identities]** | The number of identities across all audiences shared in this project for which you selected to target the profiles. |
| **[!UICONTROL Suppress identities]** | The number of identities across all audiences shared in this project for which you selected to suppress the profiles and thereby not target them in campaigns. |

-->

Innerhalb jeder Aktivität zur Zielgruppenfreigabe können Sie Informationen zu den einzelnen freigegebenen Zielgruppen abrufen.

| Metrik | Beschreibung |
|---------|----------|
| **[!UICONTROL Anzahl der Identitäten]** | Gibt die Anzahl der Profile in allen mit dieser Zielgruppe verbundenen Identitäten gemäß der neuesten Auswertung der Identitätsanzahl an. Diese Zahlen werden alle 24 Stunden aktualisiert. |
| **[!UICONTROL Identitäten überschneiden sich]** | Gibt die Anzahl der Identitäten an, die sich zwischen den Mitgliedern dieser Zielgruppe und der Gesamtpopulation der Profile im Inventar des Mitarbeiters überschneiden. |
| **[!UICONTROL Aufschlüsselung des Übereinstimmungsschlüssels]** | Zeigt die Anzahl der Identitäten für jede in der Zielgruppe verwendete Identität an. Eine Gesamtzahl von 500.000 Benutzern kann beispielsweise aus 400.000 Benutzern bestehen, die über die gehashte E-Mail-Identität und 100.000 Benutzern, die über eine Mobile-ID-Identität verschlüsselt wurden, verschlüsselt wurden. Beachten Sie, dass im hier beschriebenen Beispiel dieselbe Person mit ihrer E-Mail- und Mobile-ID-Identität möglicherweise zweimal in der Zielgruppe vorhanden ist. |
| **[!UICONTROL Ziel]** | **[!UICONTROL Unterdrücken]** oder **[!UICONTROL Ziel]**. Gibt an, ob die Mitglieder einer Zielgruppe angesprochen oder von Kampagnen ausgeschlossen werden sollen. |

Die Seite bietet auch Steuerelemente zum **[!UICONTROL (Freigabe anhalten]** und **[!UICONTROL Zielgruppen bearbeiten]**.

## Bearbeiten von Zielgruppen {#edit-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_share_edit_audiences_usecases"
>title="Anwendungsfall „Ziel“ oder „Unterdrücken“"
>abstract="<p>Wählen Sie **Ziel** aus, wenn den Profilen in der Zielgruppe in der Kampagne Anzeigen angezeigt werden sollen.</p> <p>Wählen Sie **Unterdrücken** aus, wenn Sie die Profile in der Zielgruppe vom Kampagnen-Messaging ausschließen möchten.</p>"

Wählen Sie **[!UICONTROL Zielgruppen bearbeiten]**, um zu ändern, welche Zielgruppen in einem Modul zur Freigabe von Zielgruppen freigegeben sind. Sie können auch mehrere Konfigurationen ändern, die sich auf die Freigabe von Zielgruppen beziehen.

![Ansicht des Modals „Zielgruppen bearbeiten“](/help/assets/collaborate/share/edit-audiences-modal.png)

<!--

Search for audiences that you want to add to the sharing module. 

For each audience, you can select whether you'd like to target or suppress those profiles in campaigns. 

To remove an audience from the sharing module, select the trash can icon [TODO: add spectrum icon and folder].

Select how often you would like the audience membership to be refreshed and the date range within which you want the membership of the audience to be refreshed. 

TODO: are there any limitations for frequency in the M1 release?

-->

## Nächste Schritte

Nachdem der Publisher die freigegebenen Zielgruppen erhalten hat, [ er sie jetzt ](/help/guide/collaborate/activate.md) digitalen Werbekampagnen aktivieren.
