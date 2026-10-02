---
title: Zielgruppen aktivieren
description: Erfahren Sie, wie Sie Zielgruppen senden und empfangene Zielgruppen automatisch oder manuell an Ziele in Adobe Real-Time CDP Collaboration aktivieren.
audience: admin, publisher, advertiser
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
TQID: https://experienceleague.adobe.com/bfPHtcW8Mf6RhIlg5fKcJmPSEKDyAODjbNRJ5D3SMkQ
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
    internal-label: Real-Time Customer Data Platform
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
    internal-label: Use cases
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
    internal-label: Measurement
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: df0c7fe0d09203a02a192931135abaa1715e593f
workflow-type: tm+mt
source-wordcount: '2043'
ht-degree: 2%
---
# Zielgruppen aktivieren

Verwenden Sie die **[!UICONTROL Aktivieren]**-Registerkarte innerhalb eines Projekts, um Zielgruppen an Ihren Mitarbeiter zu senden, die von Ihrem Mitarbeiter empfangenen Zielgruppen zu überprüfen und die empfangenen Zielgruppen für die Bereitstellung an ein konfiguriertes Ziel zu aktivieren. Die Aktivierung kann automatisch erstellt werden, wenn die Zielgruppe empfangen wird, oder manuell vom empfangenden Mitarbeiter. Informationen zum Konfigurieren und Verwalten von Zielen im Arbeitsbereich der obersten Ebene **[!UICONTROL Aktivierung]** finden Sie in der [Ziele - Übersicht](../destinations/overview.md).

>[!IMPORTANT]
>
>Die **[!UICONTROL Aktivieren]**-Registerkarte ist nur verfügbar, wenn der Anwendungsfall **Zielgruppenaktivierung** während [&#x200B; Verbindungsprozesses aktiviert &#x200B;](../connect/establishing-connections.md#connection-settings). Weitere Informationen zu Anwendungsfällen finden Sie unter [Verwalten von Projekten](./manage-projects.md#project-use-cases).

Verwenden Sie die [Entdecken](./discover.md), um die Zielgruppen zu identifizieren, die Ihrer Kampagne am besten entsprechen, und senden Sie sie dann an Ihren Mitarbeiter.

Wenn der Empfänger in den Verbindungseinstellungen ein Ziel für die automatische Aktivierung konfiguriert, wählt der Absender beim Senden der Zielgruppe einen Aktivierungsplan aus. Das Ziel ist für den Absender schreibgeschützt. Wenn die Zielgruppe empfangen wird, wird sie automatisch für das konfigurierte Ziel des Empfängers im Aktivierungsplan des Absenders aktiviert. Anweisungen zum Einrichten der Verbindung finden [&#x200B; unter „Konfigurieren eines Ziels für die automatische Aktivierung](../connect/manage-connections.md#configure-auto-activation-destination).

Wenn der Empfänger kein Ziel für die automatische Aktivierung konfiguriert hat, bleiben das Senden und Aktivieren separate Aktionen. Durch das Senden erhält der Empfänger Zugriff auf eine Zielgruppe, und der Empfänger wählt bei der manuellen Aktivierung ein Ziel und einen Zeitplan aus. Es können nur vorkonfigurierte Ziele für die Aktivierung innerhalb eines Projekts ausgewählt werden. Anweisungen zur Zielkonfiguration finden Sie unter [Verwalten von Zielen](../destinations/manage-destinations.md).

Die verfügbaren Abschnitte und Aktionen hängen davon ab, ob Ihre Organisation Zielgruppen im Projekt sendet oder empfängt. Die **[!UICONTROL Aktivieren]**-Registerkarte enthält die folgenden Abschnitte:

| Abschnitt | Beschreibung |
|---|---|
| **[!UICONTROL Zielgruppen an &quot;[&quot;]]** | Zielgruppen, die Sie an Ihren Mitarbeiter gesendet haben. |
| **[!UICONTROL Empfangene Zielgruppen]** | Zielgruppen, die Ihr Mitarbeiter an Sie gesendet hat und die zur Aktivierung verfügbar sind. |
| **[!UICONTROL Aktivierte Zielgruppen]** | Empfangene Zielgruppen mit automatisch oder manuell erstellten Aktivierungen. |

![Die Registerkarte Aktivieren auf Projektebene mit Zusammenfassungszahlen oben und erweiterten Abschnitten Gesendete Zielgruppen, Empfangene Zielgruppen und Aktivierte Zielgruppen . In jedem Abschnitt werden Statuszählungen und eine Tabelle mit Zielgruppendetails angezeigt.](/help/assets/collaborate/activate/activate-dashboard.png){zoomable="yes"}

## Voraussetzungen {#prerequisites}

Stellen Sie vor dem Senden oder Aktivieren von Zielgruppen Folgendes sicher:

- Zielgruppen werden bezogen und stehen zum Senden zur Verfügung. Weitere Informationen finden Sie unter [Source und Zielgruppen verwalten](../setup/onboard-audiences.md).
- Zielgruppen erfüllen den Mindestschwellenwert von 1.000 Identitätsüberschneidungen, der für das Senden und die Aktivierung erforderlich ist.
- Zielgruppen werden mit den erforderlichen Übereinstimmungsschlüsseln konfiguriert, wenn Zielgruppen mit mehreren Übereinstimmungsschlüsseln verwendet werden.
- Es ist mindestens ein Ziel konfiguriert, wenn Sie die empfangenen Zielgruppen aktivieren müssen. Weitere Informationen finden Sie unter [Ziele - Übersicht](../destinations/overview.md).
- Für die automatische Aktivierung besitzt der Empfänger ein aktives Ziel und wählt es als das [Ziel für die automatische Aktivierung](../connect/manage-connections.md#configure-auto-activation-destination) aus.

## Zielgruppen senden {#send-audiences}

Senden Sie eine Zielgruppe, um Ihrem Mitarbeiter Zugriff darauf zu gewähren. Nachdem Sie die Zielgruppe gesendet haben, wird sie im Abschnitt **[!UICONTROL Gesendete Zielgruppen an [Mitarbeiter]]** und im Abschnitt **[!UICONTROL Empfangene Zielgruppen]** Ihres Mitarbeiters angezeigt.

Navigieren Sie zu **[!UICONTROL Zusammenarbeiten]** öffnen Sie ein Projekt und wählen Sie dann die Registerkarte **[!UICONTROL Aktivieren]** aus.

Wählen Sie **[!UICONTROL Abschnitt „Gesendete Zielgruppen an [Mitarbeiter]]** das Symbol zum Hinzufügen aus (![Symbol hinzufügen.](/help/assets/icons/plus.png)). Wenn keine Zielgruppen gesendet wurden, wählen Sie stattdessen **[!UICONTROL Zielgruppe senden]** aus der leeren Anzeige aus.

![Die Registerkarte Aktivieren auf Projektebene, wenn keine Zielgruppen gesendet wurden. Die leere Meldung „Zielgruppe senden“ erklärt, dass Sie keine Zielgruppe gesendet haben, und zeigt die Schaltfläche „Zielgruppe senden“ an.](/help/assets/collaborate/activate/activate-new-audiences.png){zoomable="yes"}

Der **[!UICONTROL Zielgruppen senden]** wird geöffnet. Verwenden Sie den Zielgruppenselektor, um eine Zielgruppe zu finden, oder wählen Sie **[!UICONTROL Zielgruppen durchsuchen]** aus, um die verfügbaren Zielgruppen zu vergleichen.

>[!IMPORTANT]
>
>Nur Zielgruppen mit mehr als 1000 sich überschneidenden Identitäten können aktiviert werden. Wenn sich die Zielgruppenüberschneidungen nahe dem Identitätsschwellenwert von 1.000 befinden, kann die Aktivierung fehlschlagen.

![Der Workflow zum Senden von Zielgruppen mit einem Zielgruppenselektor und der Schaltfläche „Zielgruppen durchsuchen“. Der Workflow ermöglicht es dem Absender, eine Zielgruppe auszuwählen, bevor Übereinstimmungsschlüssel und Zugriffseinstellungen konfiguriert werden.](/help/assets/collaborate/activate/audience-activation.png){zoomable="yes"}

Überprüfen Sie im **[!UICONTROL Zielgruppen durchsuchen]** für jede Zielgruppe die **[!UICONTROL Identitätsanzahl]**, **[!UICONTROL Identitäten überschneiden]** und **[!UICONTROL Überschneidung %]**.

![Das Dialogfeld „Zielgruppen durchsuchen“ listet die verfügbaren Zielgruppen mit ihrer Identitätsanzahl, der Anzahl überlappender Identitäten und dem Überschneidungsprozentsatz auf.](/help/assets/collaborate/activate/browse-audiences.png){zoomable="yes"}

>[!IMPORTANT]
>
>Wenn eine Zielgruppe mehrere Übereinstimmungsschlüssel verwendet, muss jeder ausgewählte Übereinstimmungsschlüssel den erforderlichen Überschneidungsschwellenwert erreichen. Verwenden Sie die [Entdecken](./discover.md), um vor dem Versand zu bestätigen, dass die Zielgruppe die Überschneidungsanforderungen erfüllt.

Wählen Sie die zu sendende Audience aus und klicken Sie auf **[!UICONTROL Speichern]**.

Die ausgewählte Zielgruppe wird im Workflow mit ihren Identitäts- und Überschneidungsinformationen angezeigt.

![Der Workflow zum Senden von Zielgruppen mit einer ausgewählten Zielgruppe zeigt die Optionen Identitätsanzahl, Anzahl der sich überschneidenden Identitäten, Überschneidungsprozentsatz, Übereinstimmungsschlüssel und Übereinstimmungsschlüssel bearbeiten an.](/help/assets/collaborate/activate/audience-selected.png){zoomable="yes"}

### Übereinstimmungsschlüssel bearbeiten {#edit-match-keys}

Verwenden Sie die für die Collaborator-Verbindung konfigurierten Übereinstimmungsschlüssel oder entfernen Sie Übereinstimmungsschlüssel, die nicht für die Zielgruppe gelten.

Wählen Sie **[!UICONTROL Übereinstimmungsschlüssel bearbeiten]** in der ausgewählten Zielgruppe aus.

![Die ausgewählte Zielgruppe im Workflow „Zielgruppen senden“ mit hervorgehobener Option „Übereinstimmungsschlüssel bearbeiten“.](/help/assets/collaborate/activate/edit-match-keys.png){zoomable="yes"}

Das **[!UICONTROL Bearbeiten von Übereinstimmungsschlüsseln]** wird angezeigt. Deaktivieren Sie alle Übereinstimmungsschlüssel, die Sie nicht verwenden möchten, und wählen Sie dann **[!UICONTROL Speichern]**.

>[!NOTE]
>
>Mindestens ein Übereinstimmungsschlüssel muss ausgewählt bleiben.

![Das Dialogfeld Übereinstimmungsschlüssel bearbeiten mit Umschalter-Steuerelementen für die Übereinstimmungsschlüssel, die über die Collaborator-Verbindung und eine Schaltfläche Speichern verfügbar sind.](/help/assets/collaborate/activate/edit-match-keys-selection.png){zoomable="yes"}

### Zielgruppenzugriff konfigurieren {#configure-audience-access}

Konfigurieren Sie, wie die Zielgruppe gesendet wird und wie lange Ihr Mitarbeiter darauf zugreifen kann.

Wählen Sie mit **[!UICONTROL Steuerung]** Zugriffsdauer) eine der folgenden Optionen aus:

- **[!UICONTROL Jetzt senden (einmal)]**: Die Zielgruppe einmal senden. Der empfangende Mitwirkende kann ihn einmal aktivieren.
- **[!UICONTROL Planen eines wiederkehrenden Audience-]**: Aktualisieren Sie die Audience während eines bestimmten Zugriffszeitraums. Verwenden Sie das Steuerelement **[!UICONTROL Datumsbereich]**, um das Start- und Enddatum auszuwählen.

![Der Schritt Zugriffsdauer im Workflow Zielgruppen senden mit Optionen zum einmaligen Senden der Zielgruppe oder zum Planen eines wiederkehrenden Audience-Versands. Die Option „Wiederkehrend“ zeigt Datumssteuerelemente zum Definieren des Zugriffszeitraums an.](/help/assets/collaborate/activate/activation-frequency.png)

### Wählen eines Zeitplans für die automatische Aktivierung {#auto-activation-schedule}

Wenn Ihr Mitarbeiter ein automatisches Aktivierungsziel für die Verbindung konfiguriert hat, zeigt der Abschnitt **[!UICONTROL Aktivierung]** an, dass **[!UICONTROL Automatische Aktivierung]** aktiviert ist. Das vom Empfänger ausgewählte Ziel wird schreibgeschützt angezeigt. Verwenden Sie als Absender **[!UICONTROL Häufigkeit]**, um den Zeitpunkt der Aktivierung auszuwählen:

- **[!UICONTROL Jetzt aktivieren (einmal)]**: Führen Sie die Aktivierung einmal aus, wenn die Zielgruppe empfangen wird.
- **[!UICONTROL Einmalige Zielgruppenaktivierung planen]**: Führen Sie die Aktivierung einmal zu dem Datum und der Uhrzeit in der Zukunft aus, die Sie auswählen.
- **[!UICONTROL Wiederkehrende Aktivierung planen]**: Die Aktivierung wird für den Zeitplan ausgeführt, den Sie im ausgewählten Datumsbereich konfigurieren.

![Der Workflow „Zielgruppen senden“ mit aktivierter Option „Automatisch aktivieren“ und das Menü „Häufigkeit“ mit den Optionen für sofortige, künftige einmalige und wiederkehrende Aktivierungen.](/help/assets/collaborate/activate/choose-auto-activation-schedule.png){zoomable="yes"}

Konfigurieren Sie für eine wiederkehrende Aktivierung den Aktivierungsplan, die Startzeit und den Datumsbereich. Die automatische Aktivierung unterstützt sofortige, künftige einmalige oder wiederkehrende Zeitpläne. Wiederkehrende Zeitpläne sind nicht erforderlich.

![Der Workflow „Zielgruppen senden“ ist mit einem täglichen wiederkehrenden Aktivierungsplan, einer Startzeit und einem Datumsbereich konfiguriert.](/help/assets/collaborate/activate/configure-recurring-auto-activation.png){zoomable="yes"}

Wenn die Zielgruppe und die Zugriffseinstellungen abgeschlossen sind, wählen Sie **[!UICONTROL Senden]** aus.

Die Zielgruppe wird im Abschnitt **[!UICONTROL An [ gesendete Zielgruppen]]** angezeigt. Ihr Mitarbeiter kann sie im Abschnitt **[!UICONTROL Empfangene Zielgruppen]** überprüfen. Wenn die automatische Aktivierung aktiviert ist, erstellt Collaboration auch die Aktivierung für den Empfänger und die Aktivierung wird gemäß dem ausgewählten Zeitplan ausgeführt.

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

![Der Abschnitt Gesendete Zielgruppen mit dem Löschsymbol neben einer Zielgruppenzeile.](/help/assets/collaborate/activate/delete-sent-audiences.png){zoomable="yes"}

Ein Bestätigungsdialogfeld wird angezeigt. Klicken Sie zur Bestätigung auf **[!UICONTROL Löschen]**.

![Bestätigungsdialogfeld zum Löschen der gesendeten Zielgruppe, in dem erklärt wird, dass die Zielgruppe entfernt wird und der Mitarbeiter den Zugriff verliert, einschließlich der Schaltflächen Abbrechen und Löschen.](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

Die Zielgruppe wird aus dem Abschnitt entfernt, und Ihr Mitarbeiter verliert den Zugriff darauf.

## Empfangene Zielgruppen anzeigen {#received-audiences}

Verwenden Sie den Abschnitt **[!UICONTROL Empfangene Zielgruppen]**, um die Zielgruppen zu überprüfen, die Ihr Mitarbeiter an Sie gesendet hat. Wenn vor dem Versand der Zielgruppe ein Ziel für die automatische Aktivierung konfiguriert wurde, erstellt Collaboration automatisch eine Aktivierung, wenn die Zielgruppe empfangen wird. Für wiederkehrende automatische Aktivierungen können Sie auch eine zusätzliche manuelle Aktivierung für ein anderes Ziel erstellen. Weitere [&#x200B; finden Sie unter „Manuelles Aktivieren &#x200B;](#activate-received-audience) empfangenen Zielgruppe“. Wenn kein Ziel für die automatische Aktivierung konfiguriert wurde, aktivieren Sie die Zielgruppe manuell.

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

![Der Abschnitt Empfangene Zielgruppen mit aktiven und abgelaufenen Zielgruppengröße. In jeder Zeile für die Zielgruppe werden Name, Status, Identitätsinformationen, letzte Ausführung des Datenflusses, Zugriffsdauer, Übereinstimmungsschlüssel und ein Hinzufügen-Symbol angezeigt, das zum Starten der Aktivierung verwendet wird.](/help/assets/collaborate/activate/received-audiences-section.png){zoomable="yes"}

### Manuelles Aktivieren einer empfangenen Zielgruppe {#activate-received-audience}

Aktivieren Sie eine empfangene Zielgruppe manuell, um ihre Daten an eines Ihrer konfigurierten Ziele zu senden.

Klicken Sie **[!UICONTROL Abschnitt „Empfangene]**&quot; auf das Symbol zum Hinzufügen (![Symbol hinzufügen.](/help/assets/icons/plus.png)) neben der Zielgruppe, die Sie aktivieren möchten.

Das **[!UICONTROL Zielgruppe aktivieren]** wird angezeigt.

Verwenden Sie **[!UICONTROL Ziel]**, um das Ziel auszuwählen, das die Zielgruppendaten erhält. Wenn die Zielliste leer ist, konfigurieren Sie ein Ziel, bevor Sie fortfahren. Anweisungen finden Sie unter [Ziele - Übersicht](../destinations/overview.md).

Konfigurieren Sie die **[!UICONTROL Häufigkeit]** und die verfügbaren Zeitplansteuerelemente, um festzulegen, wann und wie oft die Aktivierung ausgeführt werden soll. Wählen Sie dann **[!UICONTROL Aktivieren]** aus.

Das folgende Beispiel zeigt den manuellen Aktivierungs-Workflow, bei **[!UICONTROL „Northstar Audience]**&quot; als Ziel ausgewählt ist.

![Ein Beispiel für das manuelle Dialogfeld „Zielgruppe aktivieren“ für Northstar Fall Campaign-Kunden, bei dem Northstar Audience Exports ausgewählt und ein täglicher Zeitplan, eine Startzeit und ein Datumsbereich konfiguriert sind.](/help/assets/collaborate/activate/manually-activate-received-audience.png){zoomable="yes"}

>[!NOTE]
>
>Für eine empfangene Zielgruppe mit wiederkehrender automatischer Aktivierung können Sie manuell eine zusätzliche Aktivierung für diese Zielgruppe an einem anderen Ziel erstellen. Die wiederkehrende automatische Aktivierung wird unabhängig voneinander fortgesetzt.

Das Dialogfeld wird geschlossen und die Aktivierung wird im Abschnitt **[!UICONTROL Aktivierte Zielgruppen]** angezeigt. Die empfangene Zielgruppe bleibt im Abschnitt **[!UICONTROL Empfangene Zielgruppen]** verfügbar, während ihr Zugriff aktiv bleibt.

## Aktivierte Zielgruppen anzeigen {#activated-audiences}

Verwenden Sie den Abschnitt **[!UICONTROL Aktivierte Zielgruppen]**, um zu bestätigen, welche empfangenen Zielgruppen automatisch oder manuell Aktivierungen erstellt haben, und überprüfen Sie ihren Ziel- und Versandstatus. Automatisch erstellte Aktivierungen werden hier angezeigt, ohne dass der Empfänger den manuellen Aktivierungs-Workflow abschließen muss.

![Die Registerkarte Aktivieren mit den Northstar Fall Campaign-Kunden in den empfangenen Zielgruppen und der automatisch erstellten täglichen Aktivierung für Northstar-Zielgruppenexporte in aktivierten Zielgruppen.](/help/assets/collaborate/activate/view-auto-activated-audience.png){zoomable="yes"}

Jede aktivierte Zielgruppe zeigt die folgenden Informationen an:

| Spalte | Beschreibung |
|---|---|
| **[!UICONTROL Zielgruppenname]** | Der Name der aktivierten Zielgruppe. |
| **[!UICONTROL Status]** | Der aktuelle Aktivierungsstatus. |
| **[!UICONTROL Anzahl aktiviert]** | Die Anzahl der für das Ziel aktivierten Identitäten. |
| **[!UICONTROL Zuletzt aktualisiert]** | Datum und Uhrzeit der letzten Aktualisierung der aktivierten Zielgruppe. |
| **[!UICONTROL Ziel]** | Das Ziel, das die Zielgruppendaten erhält. |
| **[!UICONTROL Häufigkeit]** | Die Aktivierungshäufigkeit, z. B. ein einmaliger oder ein wiederkehrender Zeitplan. |
| **[!UICONTROL Datum]** | Das Datum oder der Datumsbereich, in dem die Aktivierung ausgeführt wird. |
| **[!UICONTROL Übereinstimmungsschlüssel]** | Die in der aktivierten Zielgruppe enthaltenen Übereinstimmungsschlüssel. |

![Der Abschnitt Aktivierte Zielgruppen mit den Zahlen für aktive, archivierte und angehaltene Aktivierungen. Jede Zeile enthält den Zielgruppennamen, den Status, die aktivierte Anzahl, das Datum der letzten Aktualisierung, das Ziel, die Häufigkeit, das Aktivierungsdatum, Übereinstimmungsschlüssel und ein Löschsymbol.](/help/assets/collaborate/activate/activated-audiences-section.png){zoomable="yes"}

### Löschen einer aktivierten Zielgruppe {#delete-activated-audience}

Löschen Sie eine aktivierte Zielgruppe, um die Aktivierung aus dem Abschnitt **[!UICONTROL Aktivierte Zielgruppen]** zu entfernen.

Wählen Sie das Löschsymbol (![Löschsymbol.](/help/assets/icons/delete.png)) neben der aktivierten Zielgruppe.

Ein Bestätigungsdialogfeld wird angezeigt. Klicken Sie zur Bestätigung auf **[!UICONTROL Löschen]**.

![Das Bestätigungsdialogfeld zum Löschen aktivierter Zielgruppen , in dem erklärt wird, dass die Zielgruppe aus der Liste aktivierter Zielgruppen entfernt wird und später mit den Schaltflächen Abbrechen und Löschen erneut aktiviert werden kann.](/help/assets/collaborate/activate/delete-activated-audience-confirmation.png)

Die Aktivierung wird aus der Liste entfernt. Sie können die empfangene Zielgruppe erneut aktivieren, während ihr Zugriff aktiv bleibt.

## Nächste Schritte {#next-steps}

Überwachen Sie nach dem Senden oder Aktivieren von Zielgruppen deren Status in den Abschnitten **[!UICONTROL Gesendete Zielgruppen an [Mitarbeiter]]** und **[!UICONTROL Aktivierte Zielgruppen]** . Wenn die Kampagnen abgeschlossen sind, wenden Sie sich an das Adobe-Aktivierungs- und -Engineering-Team, um Messdaten hochzuladen und die entsprechenden [Messberichte“ &#x200B;](./measure.md).
