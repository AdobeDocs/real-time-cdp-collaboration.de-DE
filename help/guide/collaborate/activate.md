---
title: Zielgruppen aktivieren
description: Erfahren Sie, wie Sie Zielgruppen in Adobe Real-Time CDP Collaboration aktivieren.
audience: admin, publisher
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
TQID: https://experienceleague.adobe.com/bfPHtcW8Mf6RhIlg5fKcJmPSEKDyAODjbNRJ5D3SMkQ
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1016
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

Wählen Sie das Symbol hinzufügen ![Symbol hinzufügen.](/help/assets/icons/plus.png)) oder die Option **[!UICONTROL Zielgruppe aktivieren]** aus, wenn keine vorherigen Zielgruppen zur Aktivierung gesendet wurden.

![Der Arbeitsbereich „Aktivieren“ in einem Projekt ohne hinzugefügte Zielgruppen.](/help/assets/collaborate/activate/activate-new-audiences.png)

Der Workflow zum Aktivieren von Zielgruppen wird geöffnet. Dort können Sie die Zielgruppe auswählen, die Sie an Ihren Mitarbeiter senden möchten. Verwenden Sie das Dropdown-Menü, um eine Audience auszuwählen, oder suchen Sie nach einer bestimmten Audience. Um vor der Auswahl weitere Informationen zu den Zielgruppen anzuzeigen, wählen Sie **[!UICONTROL Zielgruppen durchsuchen]**

![Der Workflow für die Zielgruppenaktivierung mit hervorgehobener Dropdown-Liste und hervorgehobenen Optionen zum Durchsuchen von Zielgruppen.](/help/assets/collaborate/activate/audience-activation.png)

In **[!UICONTROL Zielgruppen durchsuchen]** werden für jede Zielgruppe die **[!UICONTROL Identitätsanzahl]**, **[!UICONTROL Identitäten überschneiden]** und **[!UICONTROL Überschneidung %]** angezeigt.

![Das Dialogfeld „Zielgruppen durchsuchen“ mit den verfügbaren Zielgruppen.](/help/assets/collaborate/activate/browse-audiences.png)

>[!IMPORTANT]
>
>Beim Aktivieren von Zielgruppen, für die mehrere Übereinstimmungsschlüssel verwendet werden, schlägt die gesamte Aktivierung fehl, wenn ein (oder mehrere) Übereinstimmungsschlüssel keine Überschneidungen, keine Zielgruppengröße oder einen Schwellenwert unterschreiten. Stellen Sie vor der Aktivierung sicher, dass sich Ihre Zielgruppen ausreichend überschneiden und der Mindestschwellenwert von 1.000 IDs für alle Übereinstimmungsschlüssel erreicht wird.

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

## Delete sent audiences {#delete-sent-audiences}

You can delete sent audiences that you no longer want to activate. When you delete a sent audience, it is removed from the **[!UICONTROL Sent audiences to]** section, and it will no longer be activated to your collaborator&#39;s destination.

To delete a sent audience, select the **[!UICONTROL Delete]** icon (![Delete icon.](/help/assets/icons/delete.png)) next to the audience in the **[!UICONTROL Sent audiences to]** section.

![The Delete option in the Sent audiences to section.](/help/assets/collaborate/activate/delete-sent-audiences.png)

A confirmation dialog opens, asking you to confirm the deletion. Klicken Sie zur Bestätigung auf **[!UICONTROL Löschen]**.

![The Delete confirmation dialog.](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

## Nächste Schritte {#next-steps}

After activating audiences and running campaigns, work with the Adobe enablement and engineering team to upload measurement data and view the corresponding [measurement reports](/help/guide/collaborate/measure.md).
