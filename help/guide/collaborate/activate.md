---
title: Zielgruppen aktivieren
description: Erfahren Sie, wie Sie Zielgruppen in Adobe Real-Time CDP Collaboration aktivieren.
audience: admin, publisher
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
source-git-commit: f19aff1b7d10a446dd209721e7a6fdf537c9d63e
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# Zielgruppen aktivieren

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>Der **[!UICONTROL Aktivieren]**-Arbeitsbereich ist nur verfügbar, wenn der Anwendungsfall **Zielgruppenaktivierung** während [ Verbindungsprozesses aktiviert ](../connect/establishing-connections.md#connection-settings). Weitere Informationen zu Anwendungsfällen finden Sie im Handbuch [Verwalten von ](./manage-projects.md#project-use-cases)&quot;.

Audience Activation ermöglicht das Aktivieren von Audiences in Kampagnen. Der Aktivierungsprozess ist eine Zusammenarbeit zwischen Werbetreibenden und Publishern. Nach [ Ermittlung der besten Zielgruppen für Ihre Kampagne ](./discover.md) Zielgruppen die Zielgruppen aktivieren. Aktivierte Zielgruppen werden an das vorkonfigurierte Ziel des Herausgebers, z. B. Adobe Experience Platform, gesendet, um sie in Kampagnen zu verwenden. Weitere Informationen zum Einrichten von Zielen finden Sie im Handbuch [Ziele - Übersicht](../destinations/overview.md).

>[!IMPORTANT]
>
>Wenn Advertiser Zielgruppen aktivieren, werden diese automatisch für das Ziel aktiviert, das der Publisher für ihre Organisation konfiguriert hat. Der Publisher **muss** ein Ziel konfigurieren *bevor* Advertiser eine Zielgruppe aktiviert. Wenn kein Ziel konfiguriert ist, wird die Zielgruppe an den Herausgeber gesendet, kann jedoch in keiner Kampagnen aktiviert werden.

## Neue Zielgruppen aktivieren

Um mit der Aktivierung von Zielgruppen zu beginnen, navigieren Sie **[!UICONTROL Registerkarte]** Aktivieren“ in Ihrem Projektarbeitsbereich.

Klicken Sie auf das Symbol Hinzufügen ![Symbol Hinzufügen .](/help/assets/icons/plus.png)) oder die Option **[!UICONTROL Zielgruppe aktivieren]** wenn keine vorherigen Zielgruppen zur Aktivierung gesendet wurden.

![Der Arbeitsbereich „Aktivieren“ in einem Projekt ohne hinzugefügte Zielgruppen.](/help/assets/collaborate/activate/activate-new-audiences.png)

Der Workflow zum Aktivieren von Zielgruppen wird geöffnet. Dort können Sie die Zielgruppe auswählen, die Sie an Ihren Mitarbeiter senden möchten. Verwenden Sie das Dropdown-Menü, um eine Audience auszuwählen, oder suchen Sie nach einer bestimmten Audience. Um vor der Auswahl weitere Informationen zu den Zielgruppen anzuzeigen, wählen Sie **[!UICONTROL Zielgruppen durchsuchen]**

![Der Workflow für die Zielgruppenaktivierung mit hervorgehobener Dropdown-Liste und hervorgehobenen Optionen zum Durchsuchen von Zielgruppen.](/help/assets/collaborate/activate/audience-activation.png)

In **[!UICONTROL Zielgruppen durchsuchen]** werden für jede Zielgruppe die **[!UICONTROL Identitätsanzahl]**, **[!UICONTROL Identitäten überschneiden]** und **[!UICONTROL Überschneidung %]** angezeigt.

![Das Dialogfeld „Zielgruppen durchsuchen“ mit den verfügbaren Zielgruppen.](/help/assets/collaborate/activate/browse-audiences.png)

Wählen Sie die Zielgruppe aus, die Sie in Kampagnen aktivieren möchten, und klicken Sie auf **[!UICONTROL Speichern]**. Die Zielgruppe wird jetzt angezeigt und Sie können die **[!UICONTROL Identitätsanzahl]**, **[!UICONTROL Überschneidende Identitäten]** und **[!UICONTROL Überschneidung %]** für die ausgewählte Zielgruppe sehen.

![Der Zielgruppen-Aktivierungs-Workflow mit der ausgewählten Zielgruppe wird angezeigt.](/help/assets/collaborate/activate/audience-selected.png)

### Übereinstimmungsschlüssel bearbeiten

Als Nächstes können Sie die Übereinstimmungsschlüssel der Zielgruppe bearbeiten, indem Sie in der ausgewählten Zielgruppe **[!UICONTROL Übereinstimmungsschlüssel bearbeiten]** auswählen. Diese Optionen werden von den ausgewählten Übereinstimmungsschlüsseln übernommen, wenn die Verbindung zwischen den Partnern eingerichtet wurde. Sie können ausgewählte Übereinstimmungsschlüssel entfernen, wenn sie nicht für eine bestimmte Kampagne gelten. Sie können jedoch keine neuen Übereinstimmungsschlüssel hinzufügen.

![Der Zielgruppen-Aktivierungs-Workflow mit der hervorgehobenen Option „Übereinstimmungsschlüssel bearbeiten“.](/help/assets/collaborate/activate/edit-match-keys.png)

Das **[!UICONTROL Bearbeiten von Übereinstimmungsschlüsseln]** wird geöffnet, in dem Sie die Übereinstimmungsschlüssel, die Sie nicht verwenden möchten, deaktivieren können. Klicken Sie **[!UICONTROL Speichern]**, um Ihre Änderungen zu speichern.

>[!NOTE]
>
>Es muss mindestens ein Übereinstimmungsschlüssel ausgewählt werden. In der aktuellen Version sind nur Übereinstimmungsschlüssel verfügbar (**[!UICONTROL -E-Mail]**, daher können Sie diesen Übereinstimmungsschlüssel nicht entfernen.

![Das Dialogfeld „Übereinstimmungsschlüssel bearbeiten“ im Zielgruppen-Aktivierungs-Workflow.](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### Festlegen der Häufigkeit und des Intervalls für die Zielgruppenaktualisierung

Legen Sie abschließend die gewünschte Häufigkeit und den gewünschten Datumsbereich für die Aktualisierung der Zielgruppe fest. In der aktuellen Version ist die einzige unterstützte Häufigkeitsoption **[!UICONTROL Einmal]**. Die Häufigkeit **[!UICONTROL Einmal]** bedeutet, dass die Zielgruppen ein einziges Mal aktiviert und nicht aktualisiert werden. Die **[!UICONTROL Datum]**-Option wird automatisch mit dem aktuellen Datum ausgefüllt.

![Der Workflow zur Zielgruppenaktivierung mit hervorgehobenem Abschnitt „Häufigkeit“.](/help/assets/collaborate/activate/audience-frequency.png)

Wenn Sie mit Ihrer Auswahl zufrieden sind, wählen Sie **[!UICONTROL Aktivieren]** aus, um den Workflow abzuschließen. Die Zielgruppe ist jetzt aktiviert und kann auf der Registerkarte **[!UICONTROL Aktivieren]** angezeigt werden. Er steht Ihren Mitwirkenden auch auf ihrer Registerkarte **[!UICONTROL Aktivieren]** zur Verfügung, wo sie ihn in Kampagnen verwenden können.

Sie können das Symbol zum Bearbeiten des Namens der Zielgruppe (![Bleistiftsymbol) bearbeiten.](/help/assets/icons/edit.png)) oder deaktivieren Sie die Zielgruppe, indem Sie **[!UICONTROL Deaktivieren]** auswählen.

![Die Registerkarte „Aktivieren“ mit der angezeigten aktivierten Zielgruppe und den hervorgehobenen Optionen „Bearbeiten“ und „Deaktivieren“.](/help/assets/collaborate/activate/edit-activate-audience.png)

## Aktivierte Zielgruppen anzeigen

Auf der Registerkarte **[!UICONTROL Aktivieren]** können sowohl Herausgeber als auch Werbetreibende die derzeit aktivierten Zielgruppen anzeigen. Derzeit werden Zielgruppen automatisch an das konfigurierte Ziel des Herausgebers gesendet, nachdem sie vom Advertiser aktiviert wurden.

![Überblick über die Registerkarte Aktivieren , auf der eine aktivierte Zielgruppe angezeigt wird.](/help/assets/collaborate/activate/activate-overview.png)

Innerhalb jeder aktivierten Zielgruppe können Sie die folgenden Metriken sehen:

| Metrik | Beschreibung |
|---------|----------|
| **[!UICONTROL Aktivierte Identitäten]** | Gibt die Anzahl der aktivierten Identitäten innerhalb der Zielgruppe an. |
| **[!UICONTROL Identitäten überschneiden sich]** | Gibt die Anzahl der Identitäten mit Überschneidungen zwischen dieser Zielgruppe und der Gesamtpopulation der Profile im Inventar des Mitarbeiters an. |
| **[!UICONTROL Aufschlüsselung des Übereinstimmungsschlüssels]** | Zeigt die Anzahl der Identitäten für jede in der Zielgruppe verwendete Identität an. Eine Gesamtzahl von 500.000 Benutzern kann beispielsweise aus 400.000 Benutzern bestehen, die über die gehashte E-Mail-Identität und 100.000 Benutzern, die über eine Mobile-ID-Identität verschlüsselt wurden, verschlüsselt wurden. Beachten Sie, dass im hier beschriebenen Beispiel dieselbe Person mit ihrer E-Mail- und Mobile-ID-Identität möglicherweise zweimal in der Zielgruppe vorhanden ist. |

## Nächste Schritte {#next-steps}

Arbeiten Sie nach der Aktivierung von Daten und der Durchführung von Kampagnen mit dem Adobe-Aktivierungs- und -Engineering-Team zusammen, um Messdaten hochzuladen und die entsprechenden [Messberichte“ ](/help/guide/collaborate/measure.md).
