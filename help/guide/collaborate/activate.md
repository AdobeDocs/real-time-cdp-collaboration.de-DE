---
title: Zielgruppen aktivieren
description: Erfahren Sie, wie Sie Zielgruppen in Adobe Real-Time CDP Collaboration aktivieren.
audience: admin, publisher
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
source-git-commit: afe8560a12017c6b993f93cde8636288aa6e4991
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 2%

---

# Zielgruppen aktivieren

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>Der **[!UICONTROL Aktivieren]**-Arbeitsbereich ist nur verfügbar, wenn der Anwendungsfall **Zielgruppenaktivierung** während [ Verbindungsprozesses aktiviert ](../connect/establishing-connections.md#connection-settings). Weitere Informationen zu Anwendungsfällen finden Sie im Handbuch [Verwalten von ](./manage-projects.md#project-use-cases)&quot;.

Mit der Zielgruppenaktivierung können Sie Zielgruppen aktivieren, um sie in Kampagnen zu verwenden. Die Aktivierung kann je nach den in der Verbindung konfigurierten Zielgruppen-Aktivierungseinstellungen [ Mitarbeiter ](/help/guide/connect/establishing-connections.md#configure-connection-settings). Nachdem Sie [die besten Audiences für Ihre Kampagne entdeckt haben](./discover.md) aktivieren Sie die Audiences, um sie für die Verwendung verfügbar zu machen. Wenn Sie eine Zielgruppe aktivieren, wird sie an das vorkonfigurierte Ziel Ihres Mitarbeiters gesendet, z. B. an Adobe Experience Platform, wo sie für die Verwendung in Kampagnen verfügbar wird. Weitere Informationen zum Einrichten von Zielen finden Sie im Handbuch [Ziele - Übersicht](../destinations/overview.md).

## Neue Zielgruppen aktivieren {#activate-new-audiences}

Um mit der Aktivierung von Zielgruppen zu beginnen, navigieren Sie **[!UICONTROL Registerkarte]** Aktivieren“ in Ihrem Projektarbeitsbereich.

>[!IMPORTANT]
>
>**Bevor** eine Zielgruppe aktivieren können, muss **Mitarbeiter** Ziel konfigurieren. Wenn Sie eine Zielgruppe aktivieren, wird sie automatisch an das konfigurierte Ziel Ihres Mitarbeiters gesendet. Wenn kein Ziel eingerichtet ist, können keine Zielgruppen aktiviert werden.
>
>![Aktivieren des Arbeitsbereichs, wenn für den Mitwirkenden kein Ziel konfiguriert ist.](/help/assets/collaborate/activate/no-destination-configured.png)

Klicken Sie auf das Symbol Hinzufügen ![Symbol Hinzufügen .](/help/assets/icons/plus.png)) oder die Option **[!UICONTROL Zielgruppe aktivieren]** wenn keine vorherigen Zielgruppen zur Aktivierung gesendet wurden.

![Der Arbeitsbereich „Aktivieren“ in einem Projekt ohne hinzugefügte Zielgruppen.](/help/assets/collaborate/activate/activate-new-audiences.png)

Der Workflow zum Aktivieren von Zielgruppen wird geöffnet. Dort können Sie die Zielgruppe auswählen, die Sie an Ihren Mitarbeiter senden möchten. Verwenden Sie das Dropdown-Menü, um eine Audience auszuwählen, oder suchen Sie nach einer bestimmten Audience. Um vor der Auswahl weitere Informationen zu den Zielgruppen anzuzeigen, wählen Sie **[!UICONTROL Zielgruppen durchsuchen]**

![Der Workflow für die Zielgruppenaktivierung mit hervorgehobener Dropdown-Liste und hervorgehobenen Optionen zum Durchsuchen von Zielgruppen.](/help/assets/collaborate/activate/audience-activation.png)

In **[!UICONTROL Zielgruppen durchsuchen]** werden für jede Zielgruppe die **[!UICONTROL Identitätsanzahl]**, **[!UICONTROL Identitäten überschneiden]** und **[!UICONTROL Überschneidung %]** angezeigt.

![Das Dialogfeld „Zielgruppen durchsuchen“ mit den verfügbaren Zielgruppen.](/help/assets/collaborate/activate/browse-audiences.png)

>[!IMPORTANT]
>
>Beim Aktivieren von Zielgruppen, für die mehrere Übereinstimmungsschlüssel verwendet werden, schlägt die gesamte Aktivierung fehl, wenn ein (oder mehrere) Übereinstimmungsschlüssel keine Überschneidungen aufweisen, keine Zielgruppen zählen oder unter den Schwellenwert fallen. Stellen Sie vor der Aktivierung sicher, dass sich Ihre Zielgruppen ausreichend überschneiden und der Mindestschwellenwert von 1.000 IDs für alle Übereinstimmungsschlüssel erreicht wird.

Wählen Sie die Zielgruppe aus, die Sie in Kampagnen aktivieren möchten, und klicken Sie auf **[!UICONTROL Speichern]**. Die Zielgruppe wird jetzt angezeigt und Sie können die **[!UICONTROL Identitätsanzahl]**, **[!UICONTROL Überschneidende Identitäten]** und **[!UICONTROL Überschneidung %]** für die ausgewählte Zielgruppe sehen.

![Der Zielgruppen-Aktivierungs-Workflow mit der ausgewählten Zielgruppe wird angezeigt.](/help/assets/collaborate/activate/audience-selected.png)

### Übereinstimmungsschlüssel bearbeiten {#edit-match-keys}

Als Nächstes können Sie die Übereinstimmungsschlüssel der Zielgruppe bearbeiten, indem Sie in der ausgewählten Zielgruppe **[!UICONTROL Übereinstimmungsschlüssel bearbeiten]** auswählen. Diese Optionen werden von den ausgewählten Übereinstimmungsschlüsseln übernommen, wenn die Verbindung zwischen den Partnern eingerichtet wurde. Sie können ausgewählte Übereinstimmungsschlüssel entfernen, wenn sie nicht für eine bestimmte Kampagne gelten. Sie können jedoch keine neuen Übereinstimmungsschlüssel hinzufügen.

![Der Zielgruppen-Aktivierungs-Workflow mit der hervorgehobenen Option „Übereinstimmungsschlüssel bearbeiten“.](/help/assets/collaborate/activate/edit-match-keys.png)

Das **[!UICONTROL Bearbeiten von Übereinstimmungsschlüsseln]** wird geöffnet, in dem Sie die Übereinstimmungsschlüssel, die Sie nicht verwenden möchten, deaktivieren können. Klicken Sie **[!UICONTROL Speichern]**, um Ihre Änderungen zu speichern.

>[!NOTE]
>
>Es muss mindestens ein Übereinstimmungsschlüssel ausgewählt werden. In der aktuellen Version sind nur Übereinstimmungsschlüssel verfügbar (**[!UICONTROL -E-Mail]**, daher können Sie diesen Übereinstimmungsschlüssel nicht entfernen.

![Das Dialogfeld „Übereinstimmungsschlüssel bearbeiten“ im Zielgruppen-Aktivierungs-Workflow.](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### Häufigkeit der Zielgruppenaktualisierung festlegen {#set-audience-refresh-frequency}

Legen Sie abschließend die gewünschte Häufigkeit und den gewünschten Datumsbereich für die Aktualisierung der Zielgruppe fest. In der aktuellen Version ist die einzige unterstützte Häufigkeitsoption **[!UICONTROL Einmal]**. Die Häufigkeit **[!UICONTROL Einmal]** bedeutet, dass die Zielgruppen ein einziges Mal aktiviert und nicht aktualisiert werden. Die **[!UICONTROL Datum]**-Option wird automatisch mit dem aktuellen Datum ausgefüllt.

![Der Workflow zur Zielgruppenaktivierung mit hervorgehobenem Abschnitt „Häufigkeit“.](/help/assets/collaborate/activate/audience-frequency.png)

Wenn Sie mit Ihrer Auswahl zufrieden sind, wählen Sie **[!UICONTROL Aktivieren]** aus, um den Workflow abzuschließen.

## Dashboard aktivieren {#activate-dashboard}

Auf der Registerkarte **[!UICONTROL Aktivieren]** können Sie alle Zielgruppen anzeigen, die an Ihren Mitarbeiter gesendet wurden, sowie alle Zielgruppen, die Ihr Mitarbeiter für Ihr Ziel aktiviert hat.

![Das Dashboard „Aktivieren“ mit den Abschnitten Gesendete Zielgruppen und Aktivierte Zielgruppen.](/help/assets/collaborate/activate/activate-dashboard.png)

## Gesendete Zielgruppen anzeigen {#view-sent-audiences}

Im Abschnitt **[!UICONTROL Gesendete Zielgruppen an]** Mitarbeiter werden alle von Ihnen gesendeten Zielgruppen aufgelistet. Derzeit werden Zielgruppen automatisch an das konfigurierte Ziel Ihres Mitarbeiters gesendet, nachdem Sie sie gesendet haben. In der Ansicht Ihres Mitarbeiters werden diese Zielgruppen im Abschnitt **[!UICONTROL Aktivierte Zielgruppen]** angezeigt.

Innerhalb jeder gesendeten Zielgruppe werden die folgenden Metriken angezeigt:

| Metrik | Beschreibung |
|---------|----------|
| **[!UICONTROL Name]** | Der Name der Zielgruppe. |
| **[!UICONTROL Status]** | Der Status der gesendeten Zielgruppe. |
| **[!UICONTROL Anzahl der Identitäten]** | Die Anzahl der Identitäten in der Zielgruppe. |
| **[!UICONTROL Identitäten überschneiden sich]** | Die Anzahl der Identitäten mit Überschneidungen zwischen dieser Zielgruppe und der Gesamtpopulation der Profile im Inventar des Mitarbeiters. |
| **[!UICONTROL Erstellt]** | Das Datum, an dem die Zielgruppe ursprünglich gesendet wurde. |
| **[!UICONTROL Zuletzt gesendet]** | Das Datum, an dem die Zielgruppe zuletzt an Ihren Mitarbeiter gesendet wurde. |
| **[!UICONTROL Übereinstimmungsschlüssel]** | Gibt den für die Zielgruppe verwendeten Übereinstimmungsschlüssel an. |

## Aktivierte Zielgruppen anzeigen {#view-activated-audiences}

Im Abschnitt **[!UICONTROL Aktivierte Zielgruppen]** können Sie alle Zielgruppen sehen, die für Ihr Ziel aktiviert wurden.

Innerhalb jeder aktivierten Zielgruppe können Sie die folgenden Metriken sehen:

| Metrik | Beschreibung |
|---------|----------|
| **[!UICONTROL Name]** | Der Name der Zielgruppe. |
| **[!UICONTROL Status]** | Der Status der aktivierten Zielgruppe. |
| **[!UICONTROL Anzahl der Identitäten]** | Die Anzahl der Identitäten, die aktiviert wurden, basierend auf den sich überschneidenden Identitäten, als Ihr Mitarbeiter die Zielgruppe gesendet hat. |
| **[!UICONTROL Erstellt]** | Das Datum, an dem die Zielgruppe aktiviert wurde. |
| **[!UICONTROL Zuletzt aktualisiert]** | Das Datum, an dem die Zielgruppe zuletzt aktualisiert wurde, basierend auf dem bei der Aktivierung ausgewählten Aktualisierungszeitplan. |
| **[!UICONTROL Ziel]** | Das Ziel, für das die Zielgruppe aktiviert wurde. |
| **[!UICONTROL Übereinstimmungsschlüssel]** | Gibt den für die Zielgruppe verwendeten Übereinstimmungsschlüssel an. |

## Gesendete Zielgruppen löschen {#delete-sent-audiences}

Gesendete Zielgruppen, die nicht mehr aktiviert werden sollen, können gelöscht werden. Wenn Sie eine gesendete Zielgruppe löschen, wird sie aus dem Abschnitt **[!UICONTROL Gesendete Zielgruppen an]** entfernt und nicht mehr für das Ziel Ihres Mitarbeiters aktiviert.

Um eine gesendete Zielgruppe zu löschen, klicken Sie auf das Symbol **[!UICONTROL Löschen]** (Symbol ![Löschen).](/help/assets/icons/delete.png)) neben der Audience im Abschnitt **[!UICONTROL Gesendete Zielgruppen an]**.

![Die Option Löschen im Abschnitt Gesendete Zielgruppen an.](/help/assets/collaborate/activate/delete-sent-audiences.png)

Ein Bestätigungsdialogfeld wird geöffnet, in dem Sie aufgefordert werden, den Löschvorgang zu bestätigen. Klicken Sie zur Bestätigung auf **[!UICONTROL Löschen]**.

![Bestätigungsdialog für das Löschen.](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

## Nächste Schritte {#next-steps}

Arbeiten Sie nach der Aktivierung von Zielgruppen und der Durchführung von Kampagnen mit dem Adobe-Aktivierungs- und -Engineering-Team zusammen, um Messdaten hochzuladen und die entsprechenden [Messberichte“ ](/help/guide/collaborate/measure.md).
