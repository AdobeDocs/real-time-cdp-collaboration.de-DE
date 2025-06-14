---
title: Datenverbindungen verwalten
description: Erfahren Sie, wie Sie in Real-Time CDP Collaboration Datenverbindungen verwalten, einschließlich Übereinstimmungsschlüsseln, Planung, Anwendungsfällen und Zielgruppenfilterung
audience: administrator, data engineer
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: b28bb5037c25f630059e6e8bc375ce28e0967ac7
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 11%

---

# Datenverbindungen verwalten

{{limited-availability-release-note}}

## Überblick

Verwenden Sie Datenverbindungen in Real-Time CDP Collaboration, um Zielgruppen aus verschiedenen Quellen zu importieren. Erfahren Sie, wie Sie Übereinstimmungsschlüssel verwalten und Datenimporte für Ihre vorhandenen Datenverbindungen planen. Darüber hinaus können Sie Zielgruppen nach verschiedenen Attributen filtern, um detailliertere Einblicke zu erhalten.

## Datenverbindungen anzeigen

Um vorhandene Datenverbindungen anzuzeigen, navigieren Sie zu **[!UICONTROL Setup]** und wählen Sie dann die Registerkarte **[!UICONTROL Meine Datenverbindungen]** aus. Es werden alle Ihre aktuellen Verbindungsdaten angezeigt, die jeweils eine kurze Übersicht enthalten. Um eine vollständige Ansicht der Informationen einer Datenverbindung zu erhalten, einschließlich der Übereinstimmungsschlüssel, Zeitplandetails und Zielgruppen, wählen Sie **[!UICONTROL Datenverbindung anzeigen]** für die entsprechende Verbindung aus.

![Arbeitsbereich einrichten, auf dem die Registerkarte „Meine Datenverbindungen“ angezeigt und hervorgehoben wird.](/help/assets/setup/manage-data-connection/my-data-connections.png){zoomable="yes"}

### Übereinstimmungsschlüssel {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="Übereinstimmungsschlüssel"
>abstract="Übereinstimmungsschlüssel bestimmen, wie Daten aus verschiedenen Quellen zugeordnet werden. Wählen Sie die Übereinstimmungsschlüssel aus, die für Ihre Anwendungsfälle und Datenschutzrichtlinien am relevantesten sind."

Übereinstimmungsschlüssel sind Kennungen, die zum zielgruppenübergreifenden Abstimmen der Mitglieder von Zielgruppen aus verschiedenen Datenquellen verwendet werden. Die Übereinstimmungsschlüssel, die Sie ursprünglich für Ihre Datenverbindung ausgewählt haben, können nicht bearbeitet werden.

>[!IMPORTANT]
> 
>Übereinstimmungsschlüssel können nach der Erstellung der Datenverbindung nicht mehr bearbeitet werden. Um Übereinstimmungsschlüssel zu aktualisieren, müssen Sie eine neue Datenverbindung erstellen.

Zu den verfügbaren Übereinstimmungsschlüsseln gehören:

- **Hash-E-Mail**

![Ein Arbeitsbereich für Datenverbindungen mit hervorgehobenem Abschnitt „Übereinstimmungsschlüssel“.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### Planung {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="Planung"
>abstract="Zeigen Sie die Planungsdetails für Ihre Datenverbindung an und bearbeiten Sie bei Bedarf die Aktualisierungshäufigkeit."

Zeigen Sie die Zeitplaneinstellungen für Ihre Datenverbindungen an und verwalten Sie sie. Die Planung bestimmt, wie oft die Zielgruppe aktualisiert wird.

Nachdem eine Datenverbindung erstellt wurde, können Sie ihre Aktualisierungshäufigkeit direkt im Abschnitt **[!UICONTROL Planung]** des Arbeitsbereichs für die Datenverbindung aktualisieren.

>[!NOTE]
>
>Beim Bezug von Zielgruppen aus Adobe Experience Platform werden Zielgruppen innerhalb von 24 Stunden nach Herstellung der Datenverbindung verfügbar. Nach dem ersten Import werden die Zielgruppendaten entsprechend der definierten Häufigkeit aktualisiert.

Weitere Informationen zur Planung finden Sie [ Abschnitt „Planung](/help/guide/setup/onboard-audiences.md#schedule) im Handbuch zum Onboarding von Zielgruppen.

![Der Arbeitsbereich einer Datenverbindung mit hervorgehobenem Abschnitt „Planung“.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

#### Zeitplan bearbeiten {#edit-scheduling}

Sie können die Häufigkeit einer vorhandenen Datenverbindung bearbeiten, um besser steuern zu können, wie oft Zielgruppen aktualisiert werden. Um den Zeitplan zu bearbeiten, wählen Sie **[!UICONTROL Bearbeiten]** in der Datenverbindung auf der Planungskarte aus.

Wählen Sie **[!UICONTROL Dialogfeld &quot;]**&quot; das Dropdown-Menü aus, um die **[!UICONTROL Häufigkeit]** zu aktualisieren. Stellen Sie die Aktualisierungshäufigkeit so ein, dass sie täglich oder alle zwei bis sechs Tage ausgeführt wird. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Speichern]**, um Ihre Änderungen anzuwenden.

![Das Dialogfeld Planung mit Optionen zum Festlegen von Häufigkeit und Datumsbereich.](../../assets/setup/manage-data-connection/scheduling-dialog.png){zoomable="yes" alt="The Scheduling dialog with editable fields for frequency."}

## Datenverbindung löschen

Durch das Löschen einer Datenverbindung werden alle zugrunde liegenden Zielgruppen, zugehörigen Einstellungen und die Nutzung in der gesamten Plattform entfernt. Diese Aktion kann nicht rückgängig gemacht werden.

Um eine vorhandene Datenverbindung zu löschen, wählen Sie das Löschsymbol (![Löschsymbol) ](/help/assets/common/delete.svg) Arbeitsbereich einer einzelnen Datenverbindung aus.

![Ein Arbeitsbereich für Datenverbindungen mit hervorgehobener Löschoption.](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

Ein Bestätigungsdialogfeld wird angezeigt. Wählen Sie **[!UICONTROL Löschen]** aus, um das Löschen der Datenverbindung abzuschließen.

![Das Dialogfeld „Datenverbindung löschen“ mit hervorgehobener Option „Löschen“.](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## Verwalten von Zielgruppen {#manage-audiences}

Unten im Arbeitsbereich wird eine Liste von Audiences angezeigt, die mit der Datenverbindung verbunden sind. Die Liste zeigt einen kurzen Überblick über jede Zielgruppe, einschließlich ihres Status, ihrer Quelle und ihres Verbindungszugriffs. Um die Kategorien, den Verbindungszugriff oder die Sichtbarkeit der Metadaten einer Zielgruppe zu bearbeiten, wählen Sie den Namen der Zielgruppe aus. Eine vollständige Anleitung zum Verwalten einer Zielgruppe finden Sie im [Anzeigen einzelner Zielgruppen](./onboard-audiences.md#view-individual-audiences).

![Ein Arbeitsbereich für Datenverbindungen mit hervorgehobenen Zielgruppen.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## Nächste Schritte

Nach der Verwaltung Ihrer Datenverbindungen können Sie [Überschneidungen](/help/guide/collaborate/discover.md) zwischen Ihren Zielgruppen und den Zielgruppen entdecken, die Ihr Mitarbeiter entdeckt hat.
