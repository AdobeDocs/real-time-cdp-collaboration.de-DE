---
title: Zielgruppen aktivieren
description: Erfahren Sie, wie Sie Zielgruppen an Mitwirkende senden und die empfangenen Zielgruppen manuell aktivieren können, um Ziele in Adobe Real-Time CDP Collaboration zu erreichen.
audience: admin, publisher, advertiser
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
TQID: https://experienceleague.adobe.com/bfPHtcW8Mf6RhIlg5fKcJmPSEKDyAODjbNRJ5D3SMkQ
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 5d12a5004a6854392c130fd6b93a841fb22cf6ab
workflow-type: tm+mt
source-wordcount: 1565
ht-degree: 2%

---

# Zielgruppen aktivieren

Verwenden Sie die **[!UICONTROL Aktivieren]**-Registerkarte innerhalb eines Projekts, um Zielgruppen an Ihren Mitarbeiter zu senden, die von Ihrem Mitarbeiter empfangenen Zielgruppen zu überprüfen und die empfangenen Zielgruppen für die Bereitstellung an ein konfiguriertes Ziel zu aktivieren. Informationen zum Konfigurieren und Verwalten von Zielen im Arbeitsbereich der obersten Ebene **[!UICONTROL Aktivierung]** finden Sie in der [Ziele - Übersicht](../destinations/overview.md).

>[!IMPORTANT]
>
>Die **[!UICONTROL Aktivieren]**-Registerkarte ist nur verfügbar, wenn der Anwendungsfall **Zielgruppenaktivierung** während [ Verbindungsprozesses aktiviert ](../connect/establishing-connections.md#connection-settings). Weitere Informationen zu Anwendungsfällen finden Sie unter [Verwalten von Projekten](./manage-projects.md#project-use-cases).

Verwenden Sie die [Entdecken](./discover.md), um die Zielgruppen zu identifizieren, die Ihrer Kampagne am besten entsprechen, und senden Sie sie dann an Ihren Mitarbeiter. Der empfangende Mitarbeiter wählt ein konfiguriertes Ziel aus und plant die empfangene Audience für die Aktivierung.

Senden und Aktivieren sind separate Aktionen. Durch das Senden erhält der/die Mitwirkende Zugriff auf eine Zielgruppe. Der empfangende Mitarbeiter wählt dann ein Ziel aus und aktiviert die empfangene Zielgruppe manuell.

Die verfügbaren Abschnitte und Aktionen hängen davon ab, ob Ihre Organisation Zielgruppen im Projekt sendet oder empfängt. Die **[!UICONTROL Aktivieren]**-Registerkarte enthält die folgenden Abschnitte:

| Abschnitt | Beschreibung |
|---|---|
| **[!UICONTROL Zielgruppen an &quot;[&quot;]]** | Zielgruppen, die Sie an Ihren Mitarbeiter gesendet haben. |
| **[!UICONTROL Empfangene Zielgruppen]** | Zielgruppen, die Ihr Mitarbeiter an Sie gesendet hat und die zur Aktivierung verfügbar sind. |
| **[!UICONTROL Aktivierte Zielgruppen]** | Sie haben Zielgruppen erhalten, die Sie für ein Ziel aktiviert haben. |

![Die Registerkarte Aktivieren auf Projektebene mit Zusammenfassungszahlen oben und erweiterten Abschnitten Gesendete Zielgruppen, Empfangene Zielgruppen und Aktivierte Zielgruppen . In jedem Abschnitt werden Statuszählungen und eine Tabelle mit Zielgruppendetails angezeigt.](/help/assets/collaborate/activate/activate-dashboard.png)

## Voraussetzungen {#prerequisites}

Stellen Sie vor dem Senden oder Aktivieren von Zielgruppen Folgendes sicher:

- Zielgruppen werden bezogen und stehen zum Senden zur Verfügung. Weitere Informationen finden Sie unter [Source und Zielgruppen verwalten](../setup/onboard-audiences.md).
- Es ist mindestens ein Ziel konfiguriert, wenn Sie die empfangenen Zielgruppen aktivieren müssen. Weitere Informationen finden Sie unter [Ziele - Übersicht](../destinations/overview.md).

## Zielgruppen senden {#send-audiences}

Senden Sie eine Zielgruppe, um Ihrem Mitarbeiter Zugriff darauf zu gewähren. Nachdem Sie die Zielgruppe gesendet haben, wird sie im Abschnitt **[!UICONTROL Gesendete Zielgruppen an [Mitarbeiter]]** und im Abschnitt **[!UICONTROL Empfangene Zielgruppen]** Ihres Mitarbeiters angezeigt.

Navigieren Sie zu **[!UICONTROL Zusammenarbeiten]** öffnen Sie ein Projekt und wählen Sie dann die Registerkarte **[!UICONTROL Aktivieren]** aus.

Wählen Sie **[!UICONTROL Abschnitt „Gesendete Zielgruppen an [Mitarbeiter]]** das Symbol zum Hinzufügen aus (![Symbol hinzufügen.](/help/assets/icons/plus.png)). Wenn keine Zielgruppen gesendet wurden, wählen Sie stattdessen **[!UICONTROL Zielgruppe senden]** aus der leeren Anzeige aus.

![Die Registerkarte Aktivieren auf Projektebene, wenn keine Zielgruppen gesendet wurden. Die leere Meldung „Zielgruppe senden“ erklärt, dass Sie keine Zielgruppe gesendet haben, und zeigt die Schaltfläche „Zielgruppe senden“ an.](/help/assets/collaborate/activate/activate-new-audiences.png)

Der **[!UICONTROL Zielgruppen senden]** wird geöffnet. Verwenden Sie den Zielgruppenselektor, um eine Zielgruppe zu finden, oder wählen Sie **[!UICONTROL Zielgruppen durchsuchen]** aus, um die verfügbaren Zielgruppen zu vergleichen.

![Der Workflow zum Senden von Zielgruppen mit einem Zielgruppenselektor und der Schaltfläche „Zielgruppen durchsuchen“. Der Workflow ermöglicht es dem Absender, eine Zielgruppe auszuwählen, bevor Übereinstimmungsschlüssel und Zugriffseinstellungen konfiguriert werden.](/help/assets/collaborate/activate/audience-activation.png)

Überprüfen Sie im **[!UICONTROL Zielgruppen durchsuchen]** für jede Zielgruppe die **[!UICONTROL Identitätsanzahl]**, **[!UICONTROL Identitäten überschneiden]** und **[!UICONTROL Überschneidung %]**.

![Das Dialogfeld „Zielgruppen durchsuchen“ listet die verfügbaren Zielgruppen mit ihrer Identitätsanzahl, der Anzahl überlappender Identitäten und dem Überschneidungsprozentsatz auf.](/help/assets/collaborate/activate/browse-audiences.png)

>[!IMPORTANT]
>
>Wenn eine Zielgruppe mehrere Übereinstimmungsschlüssel verwendet, muss jeder ausgewählte Übereinstimmungsschlüssel den erforderlichen Überschneidungsschwellenwert erreichen. Verwenden Sie die [Entdecken](./discover.md), um vor dem Versand zu bestätigen, dass die Zielgruppe die Überschneidungsanforderungen erfüllt.

Wählen Sie die zu sendende Audience aus und klicken Sie auf **[!UICONTROL Speichern]**.

Die ausgewählte Zielgruppe wird im Workflow mit ihren Identitäts- und Überschneidungsinformationen angezeigt.

![Der Workflow zum Senden von Zielgruppen mit einer ausgewählten Zielgruppe zeigt die Optionen Identitätsanzahl, Anzahl der sich überschneidenden Identitäten, Überschneidungsprozentsatz, Übereinstimmungsschlüssel und Übereinstimmungsschlüssel bearbeiten an.](/help/assets/collaborate/activate/audience-selected.png)

### Übereinstimmungsschlüssel bearbeiten {#edit-match-keys}

Verwenden Sie die für die Collaborator-Verbindung konfigurierten Übereinstimmungsschlüssel oder entfernen Sie Übereinstimmungsschlüssel, die nicht für die Zielgruppe gelten.

Wählen Sie **[!UICONTROL Übereinstimmungsschlüssel bearbeiten]** in der ausgewählten Zielgruppe aus.

![Die ausgewählte Zielgruppe im Workflow „Zielgruppen senden“ mit hervorgehobener Option „Übereinstimmungsschlüssel bearbeiten“.](/help/assets/collaborate/activate/edit-match-keys.png)

Das **[!UICONTROL Bearbeiten von Übereinstimmungsschlüsseln]** wird angezeigt. Deaktivieren Sie alle Übereinstimmungsschlüssel, die Sie nicht verwenden möchten, und wählen Sie dann **[!UICONTROL Speichern]**.

>[!NOTE]
>
>Mindestens ein Übereinstimmungsschlüssel muss ausgewählt bleiben.

![Das Dialogfeld Übereinstimmungsschlüssel bearbeiten mit Umschalter-Steuerelementen für die Übereinstimmungsschlüssel, die über die Collaborator-Verbindung und eine Schaltfläche Speichern verfügbar sind.](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### Zielgruppenzugriff konfigurieren {#configure-audience-access}

Konfigurieren Sie, wie die Zielgruppe gesendet wird und wie lange Ihr Mitarbeiter darauf zugreifen kann.

Wählen Sie mit **[!UICONTROL Steuerung]** Zugriffsdauer) eine der folgenden Optionen aus:

- **[!UICONTROL Jetzt senden (einmal)]**: Die Zielgruppe einmal senden. Der empfangende Mitwirkende kann ihn einmal aktivieren.
- **[!UICONTROL Planen eines wiederkehrenden Audience-]**: Aktualisieren Sie die Audience während eines bestimmten Zugriffszeitraums. Verwenden Sie das Steuerelement **[!UICONTROL Datumsbereich]**, um das Start- und Enddatum auszuwählen.

![Der Schritt Zugriffsdauer im Workflow Zielgruppen senden mit Optionen zum einmaligen Senden der Zielgruppe oder zum Planen eines wiederkehrenden Audience-Versands. Die Option „Wiederkehrend“ zeigt Datumssteuerelemente zum Definieren des Zugriffszeitraums an.](/help/assets/collaborate/activate/activation-frequency.png)

Wenn die Zielgruppe und die Zugriffseinstellungen abgeschlossen sind, wählen Sie **[!UICONTROL Senden]** aus.

Die Zielgruppe wird im Abschnitt **[!UICONTROL An [ gesendete Zielgruppen]]** angezeigt. Ihr Mitarbeiter kann sie im Abschnitt **[!UICONTROL Empfangene Zielgruppen]** überprüfen.

## Gesendete Zielgruppen anzeigen {#view-sent-audiences}

Verwenden Sie den Abschnitt **[!UICONTROL Gesendete Zielgruppen an [Mitarbeiter]]**, um von Ihnen gesendete Zielgruppen zu überprüfen und ihren aktuellen Zugriffsstatus zu überwachen.

Für jede gesendete Zielgruppe werden die folgenden Informationen angezeigt:

| Spalte | Beschreibung |
|---|---|
| **[!UICONTROL Zielgruppenname]** | Der Name der gesendeten Zielgruppe. |
| **[!UICONTROL Status]** | Der aktuelle Zugriffsstatus der Zielgruppe. |
| **[!UICONTROL Anzahl der Identitäten]** | Die Anzahl der Identitäten in der Zielgruppe. |
| **[!UICONTROL Identitäten überschneiden sich]** | Die Anzahl der Identitäten, die sich mit dem Inventar Ihres Mitarbeiters überschneiden. |
| **[!UICONTROL Erstellt]** | Datum und Uhrzeit des ersten Versands der Zielgruppe. |
| **[!UICONTROL Zuletzt gesendet]** | Das Datum und die Uhrzeit, zu der Zielgruppendaten zuletzt an Ihren Mitarbeiter gesendet wurden. |
| **[!UICONTROL Zugriffsdauer]** | Die Zugriffseinstellung, die beim Senden der Zielgruppe konfiguriert wurde. |
| **[!UICONTROL Übereinstimmungsschlüssel]** | Die beim Senden der Zielgruppe verwendeten Übereinstimmungsschlüssel. |

### Gesendete Zielgruppe löschen {#delete-sent-audience}

Löschen Sie eine gesendete Zielgruppe, um sie aus der Liste der gesendeten Zielgruppen zu entfernen und den Zugriff Ihres Mitarbeiters zu widerrufen.

Wählen Sie das Löschsymbol (![Löschsymbol.](/help/assets/icons/delete.png)) neben der Audience im Abschnitt **[!UICONTROL Gesendete Zielgruppen an [Mitarbeiter]]**.

![Der Abschnitt Gesendete Zielgruppen mit dem Löschsymbol neben einer Zielgruppenzeile.](/help/assets/collaborate/activate/delete-sent-audiences.png)

Ein Bestätigungsdialogfeld wird angezeigt. Klicken Sie zur Bestätigung auf **[!UICONTROL Löschen]**.

![Bestätigungsdialogfeld zum Löschen der gesendeten Zielgruppe, in dem erklärt wird, dass die Zielgruppe entfernt wird und der Mitarbeiter den Zugriff verliert, einschließlich der Schaltflächen Abbrechen und Löschen.](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

Die Zielgruppe wird aus dem Abschnitt entfernt, und Ihr Mitarbeiter verliert den Zugriff darauf.

## Empfangene Zielgruppen anzeigen {#received-audiences}

Verwenden Sie den Abschnitt **[!UICONTROL Empfangene Zielgruppen]**, um die Zielgruppen zu überprüfen, die Ihr Mitarbeiter an Sie gesendet hat. Eine empfangene Zielgruppe muss manuell aktiviert werden, bevor ihre Daten an ein Ziel gesendet werden.

Jede empfangene Zielgruppe zeigt die folgenden Informationen an:

| Spalte | Beschreibung |
|---|---|
| **[!UICONTROL Zielgruppenname]** | Der Name der empfangenen Zielgruppe. |
| **[!UICONTROL Status]** | Der aktuelle Zugriffsstatus der Zielgruppe. |
| **[!UICONTROL Anzahl der Identitäten]** | Die Anzahl der Identitäten in der Zielgruppe. |
| **[!UICONTROL Identitäten überschneiden sich]** | Die Anzahl der Identitäten, die sich mit Ihrem Inventar überschneiden. |
| **[!UICONTROL Letzte Datenflussausführung]** | Datum und Uhrzeit der letzten Datenflussausführung für die Zielgruppe. |
| **[!UICONTROL Zugriffsdauer]** | Die Zugriffseinstellung, die vom Mitarbeiter konfiguriert wurde, der die Zielgruppe gesendet hat. |
| **[!UICONTROL Übereinstimmungsschlüssel]** | Die für die Zielgruppe verwendeten Übereinstimmungsschlüssel. |

![Der Abschnitt Empfangene Zielgruppen mit aktiven und abgelaufenen Zielgruppengröße. In jeder Zeile für die Zielgruppe werden Name, Status, Identitätsinformationen, letzte Ausführung des Datenflusses, Zugriffsdauer, Übereinstimmungsschlüssel und ein Hinzufügen-Symbol angezeigt, das zum Starten der Aktivierung verwendet wird.](/help/assets/collaborate/activate/received-audiences-section.png)

### Aktivieren einer empfangenen Zielgruppe {#activate-received-audience}

Aktivieren Sie eine empfangene Zielgruppe, um ihre Daten an eines Ihrer konfigurierten Ziele zu senden.

Klicken Sie **[!UICONTROL Abschnitt „Empfangene]**&quot; auf das Symbol zum Hinzufügen (![Symbol hinzufügen.](/help/assets/icons/plus.png)) neben der Zielgruppe, die Sie aktivieren möchten.

Das **[!UICONTROL Zielgruppe aktivieren]** wird angezeigt.

Verwenden Sie **[!UICONTROL Ziel]**, um das Ziel auszuwählen, das die Zielgruppendaten erhält. Wenn die Zielliste leer ist, konfigurieren Sie ein Ziel, bevor Sie fortfahren. Anweisungen finden Sie unter [Ziele - Übersicht](../destinations/overview.md).

Wählen Sie **[!UICONTROL Datum]** das Datum aus, an dem die Aktivierung ausgeführt wird, und wählen Sie dann **[!UICONTROL Aktivieren]** aus.

![Das Dialogfeld „Zielgruppe aktivieren“ wurde von einer empfangenen Zielgruppe aus geöffnet. Das Dialogfeld enthält ein Ziel-Dropdown-Menü zur Auswahl eines konfigurierten Ziels, ein Datumsfeld mit einem Kalendersteuerelement sowie die Schaltflächen Abbrechen und Aktivieren ](/help/assets/collaborate/activate/activate-received-audience.png)

Das Dialogfeld wird geschlossen und die Aktivierung wird im Abschnitt **[!UICONTROL Aktivierte Zielgruppen]** angezeigt. Die empfangene Zielgruppe bleibt im Abschnitt **[!UICONTROL Empfangene Zielgruppen]** verfügbar, während ihr Zugriff aktiv bleibt.

## Aktivierte Zielgruppen anzeigen {#activated-audiences}

Verwenden Sie den Abschnitt **[!UICONTROL Aktivierte Zielgruppen]**, um zu bestätigen, welche empfangenen Zielgruppen aktiviert wurden, und um ihren Ziel- und Versandstatus zu überprüfen.

Jede aktivierte Zielgruppe zeigt die folgenden Informationen an:

| Spalte | Beschreibung |
|---|---|
| **[!UICONTROL Zielgruppenname]** | Der Name der aktivierten Zielgruppe. |
| **[!UICONTROL Status]** | Der aktuelle Aktivierungsstatus. |
| **[!UICONTROL Anzahl aktiviert]** | Die Anzahl der für das Ziel aktivierten Identitäten. |
| **[!UICONTROL Zuletzt aktualisiert]** | Datum und Uhrzeit der letzten Aktualisierung der aktivierten Zielgruppe. |
| **[!UICONTROL Ziel]** | Das Ziel, das die Zielgruppendaten erhält. |
| **[!UICONTROL Häufigkeit]** | Die Aktivierungsfrequenz. Manuelle Aktivierungen werden **[!UICONTROL einmal]** angezeigt. |
| **[!UICONTROL Datum]** | Das Datum, an dem die Aktivierung ausgeführt wird. |
| **[!UICONTROL Übereinstimmungsschlüssel]** | Die in der aktivierten Zielgruppe enthaltenen Übereinstimmungsschlüssel. |

![Der Abschnitt Aktivierte Zielgruppen mit den Zahlen für aktive, archivierte und angehaltene Aktivierungen. Jede Zeile enthält den Zielgruppennamen, den Status, die aktivierte Anzahl, das Datum der letzten Aktualisierung, das Ziel, die Häufigkeit, das Aktivierungsdatum, Übereinstimmungsschlüssel und ein Löschsymbol.](/help/assets/collaborate/activate/activated-audiences-section.png)

### Löschen einer aktivierten Zielgruppe {#delete-activated-audience}

Löschen Sie eine aktivierte Zielgruppe, um die Aktivierung aus dem Abschnitt **[!UICONTROL Aktivierte Zielgruppen]** zu entfernen.

Wählen Sie das Löschsymbol (![Löschsymbol.](/help/assets/icons/delete.png)) neben der aktivierten Zielgruppe.

Ein Bestätigungsdialogfeld wird angezeigt. Klicken Sie zur Bestätigung auf **[!UICONTROL Löschen]**.

![Das Bestätigungsdialogfeld zum Löschen aktivierter Zielgruppen , in dem erklärt wird, dass die Zielgruppe aus der Liste aktivierter Zielgruppen entfernt wird und später mit den Schaltflächen Abbrechen und Löschen erneut aktiviert werden kann.](/help/assets/collaborate/activate/delete-activated-audience-confirmation.png)

Die Aktivierung wird aus der Liste entfernt. Sie können die empfangene Zielgruppe erneut aktivieren, während ihr Zugriff aktiv bleibt.

## Nächste Schritte {#next-steps}

Überwachen Sie nach dem Senden oder Aktivieren von Zielgruppen deren Status in den Abschnitten **[!UICONTROL Gesendete Zielgruppen an [Mitarbeiter]]** und **[!UICONTROL Aktivierte Zielgruppen]** . Wenn die Kampagnen abgeschlossen sind, wenden Sie sich an das Adobe-Aktivierungs- und -Engineering-Team, um Messdaten hochzuladen und die entsprechenden [Messberichte“ ](./measure.md).
