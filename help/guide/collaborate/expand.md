---
title: Erstellen von Erweiterungszielgruppen in „Erweitern“
description: Erfahren Sie, wie Sie mithilfe der Zielgruppenpopulation eines Mitarbeiters in Adobe Real-Time CDP Collaboration Erweiterungszielgruppen aus einer Seed-Zielgruppe erstellen.
source-git-commit: d2585628407acf10ad8388231259c77991a9a0b0
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 2%
---
# (Beta) Erstellen von Erweiterungszielgruppen unter „Erweitern“

Verwenden Sie die **[!UICONTROL Erweitern]** in einem Projekt, um eine Erweiterungszielgruppe aus einer Ihrer Zielgruppen zu erstellen. Collaboration verwendet die Zielgruppenpopulation Ihres Mitarbeiters, um Profile zu finden, die Ihrer Seed-Zielgruppe ähneln, sodass Sie neue potenzielle Kunden erreichen können, ohne die zugrunde liegenden Zielgruppendaten Ihres Mitarbeiters offenzulegen. Die resultierende Erweiterungszielgruppe wird zur Aktivierung an Ihren Mitarbeiter gesendet.

## Voraussetzungen {#prerequisites}

Bevor Sie die Registerkarte **[!UICONTROL Erweitern]** verwenden können, sollten Sie über Folgendes verfügen:

* [Sourced](/help/guide/setup/onboard-audiences.md) mindestens eine Zielgruppe, die als Seed-Zielgruppe verwendet werden soll
* [Verbunden](/help/guide/connect/establishing-connections.md) mit einem Mitarbeiter
* [hat ein Projekt ](/help/guide/collaborate/manage-projects.md) diesem Mitarbeiter erstellt
* Wenn Sie eine Erweiterungszielgruppe erhalten, ein [Ziel](/help/guide/destinations/overview.md), das für den Empfang aktivierter Zielgruppen konfiguriert ist

## Übersicht erweitern {#expand-overview}

Navigieren Sie zu **[!UICONTROL Zusammenarbeiten]** > **[!UICONTROL Meine Projekte]**, öffnen Sie ein Projekt und wählen Sie die Registerkarte **[!UICONTROL Erweitern]** aus.

Auf **[!UICONTROL Seite &quot;]**&quot; werden die für diesen Mitarbeiter erstellten Erweiterungszielgruppen und die Option zum Erstellen einer neuen Zielgruppe angezeigt.

![Die Registerkarte „Erweitern“, auf der die Tabelle „Erweitern von Zielgruppen“ mit den Spalten „Name“, „Status“, „Modellgröße“, „Reichweite der Zielgruppe“ und „Zuletzt aktualisiert“ angezeigt wird.](/help/assets/collaborate/expand/expand-overview.png){zoomable="yes"}

In **[!UICONTROL Tabelle &quot;]**&quot; werden alle im Projekt erstellten Erweiterungszielgruppen aufgelistet:

| Spalte | Beschreibung |
|---|---|
| **[!UICONTROL Name]** | Der Name der Erweiterungszielgruppe. Standardmäßig wird der Name der Seed-Zielgruppe verwendet, bis er bearbeitet wird. |
| **[!UICONTROL Status]** | Der aktuelle Status der Audience-Erweiterung. Siehe [Erweiterung des Zielgruppenstatus](#expansion-audience-status) für Details. |
| **[!UICONTROL Modellgröße]** | Die Größe der generierten Erweiterungszielgruppe. Diese Option ist erst nach Abschluss der Modellverarbeitung verfügbar. |
| **[!UICONTROL Audience-Reichweite]** | Die Einstellung „Zielgruppenreichweite“, die für die Erweiterung der Zielgruppe verwendet wird. |
| **[!UICONTROL Zuletzt aktualisiert]** | Datum und Uhrzeit der letzten Aktualisierung der Erweiterungszielgruppe. |

{style="table-layout:auto"}

### Audience-Status erweitern {#expansion-audience-status}

Eine Erweiterungszielgruppe durchläuft die folgenden Status:

| Status | Beschreibung |
|---|---|
| **[!UICONTROL Verarbeitung läuft]** | Das Erweiterungsmodell generiert weiterhin die Erweiterungszielgruppe. |
| **[!UICONTROL Entwurf]** | Das Modell ist fertig, und die Zielgruppe für die Erweiterung kann überprüft und an Ihren Mitarbeiter gesendet werden. |
| **[!UICONTROL Aktiv]** | Sie haben die Erweiterungszielgruppe an Ihren Mitarbeiter gesendet. |

{style="table-layout:auto"}

>[!NOTE]
>
>Der Status wird nicht in Echtzeit aktualisiert. Öffnen oder aktualisieren Sie die Registerkarte **[!UICONTROL Erweitern]**, um den neuesten Status anzuzeigen.

## Erstellen einer Audience für die Erweiterung {#create-expansion-audience}

Um eine neue Audience-Erweiterung zu erstellen, klicken Sie auf das Symbol zum Hinzufügen (![Symbol hinzufügen.](/help/assets/icons/plus.png)) Klicken Sie auf **[!UICONTROL Seite &quot;]**&quot; auf **[!UICONTROL Erweiterte Zielgruppe erstellen]**.


Das **[!UICONTROL Erweiterungszielgruppe generieren]** wird angezeigt. Füllen Sie jedes Feld aus, um die Audience für die Erweiterung zu generieren.

![Das Dialogfeld „Zielgruppenerweiterung generieren“ mit den Feldern „Seed-Zielgruppe“, „Zielgruppenreichweite“, „Übereinstimmungsschlüssel“ und „Seed-Zielgruppenmitglieder“.](/help/assets/collaborate/expand/generate-expansion-audience-dialog.png){zoomable="yes"}

### Auswählen der Seed-Zielgruppe {#select-seed-audience}

Wählen Sie eine Ihrer eigenen Zielgruppen aus der Dropdown-Liste **[!UICONTROL Wählen Sie Ihre Seed-Zielgruppe]** aus. Collaboration verwendet diese Zielgruppe als Grundlage für die Suche nach ähnlichen Profilen in der Population Ihres Mitarbeiters.

![Das Feld Seed-Zielgruppe im Dialogfeld „Erweiterung der Zielgruppe generieren“.](/help/assets/collaborate/expand/select-seed-audience.png){zoomable="yes"}

### Übereinstimmungsschlüssel auswählen {#select-match-key}

Aktivieren Sie einen Übereinstimmungsschlüssel für die Erweiterungszielgruppe. Sie können nicht mehr als eine aktivieren.

| Personen-IDs | Geräte-IDs |
|---|---|
| **[!UICONTROL Hash-E-Mail]** | **[!UICONTROL Hash-IPv4]** |
| **[!UICONTROL Hash-Telefon]** | **[!UICONTROL GAID]** |
| **[!UICONTROL Treue-ID]** | **[!UICONTROL IDFA]** |
| **[!UICONTROL CRM-ID]** | **[!UICONTROL demdex-ID]** |

{style="table-layout:auto"}

>[!NOTE]
>
>Wenn Ihre Seed-Zielgruppe keinen bestimmten Übereinstimmungsschlüssel enthält, wird diese Option deaktiviert angezeigt und kann nicht ausgewählt werden.

![Der Abschnitt „Übereinstimmungsschlüssel“ im Dialogfeld „Zielgruppenerweiterung generieren“ mit den verfügbaren Übereinstimmungsschlüsseloptionen.](/help/assets/collaborate/expand/select-match-key.png){zoomable="yes"}

### Auswählen der Reichweite Ihrer Audience {#select-audience-reach}

Verwenden Sie das **[!UICONTROL Zielgruppenreichweite]**, um die Ähnlichkeit mit Ihrer Seed-Zielgruppe und die Reichweite insgesamt in Einklang zu bringen. Wählen Sie **[!UICONTROL Ausbalanciert]** aus, um einen Mittelweg zwischen der Ähnlichkeit mit Ihrer Seed-Zielgruppe und der Gesamtreichweite zu finden.

![Das Feld „Audience-Reichweite“ im Dialogfeld „Audience-Erweiterung generieren“ mit ausgewählter Option „Ausgeglichen“ und dem darunter liegenden Beschreibungstext.](/help/assets/collaborate/expand/select-audience-reach.png){zoomable="yes"}

### Ein- oder Ausschließen der Seed-Zielgruppe {#include-exclude-seed-audience}

Verwenden Sie die Optionsfelder **[!UICONTROL Seed]** Zielgruppe, um auszuwählen, ob Ihre ursprüngliche Seed-Zielgruppe in die Zielgruppe der endgültigen Erweiterung eingeschlossen oder davon ausgeschlossen werden soll.

![Das Feld Seed-Zielgruppenmitglieder im Dialogfeld Zielgruppenerweiterung generieren mit den Optionsfeldern Ja und Nein.](/help/assets/collaborate/expand/include-exclude-seed-audience.png){zoomable="yes"}

### Zielgruppe für die Erweiterung generieren {#generate-expansion-audience}

Nachdem alle Felder ausgefüllt sind, wählen Sie **[!UICONTROL Zielgruppe erweitern]** aus. Eine Bestätigungsmeldung bestätigt, dass Collaboration die Erweiterungszielgruppe erstellt und dass Sie deren Fortschritt auf der Seite **[!UICONTROL Erweitern]** verfolgen können.

## Überprüfen und Senden einer Erweiterungszielgruppe {#review-send-expansion-audience}

Sobald der Status einer Erweiterungszielgruppe auf „Entwurf **[!UICONTROL aktualisiert wurde]** wählen Sie ihren Namen in der Tabelle **[!UICONTROL Erweiterungszielgruppen]** aus, um sie zu öffnen.

![Die Detailseite „Zielgruppe erweitern“ mit den Zielgruppen-Metadaten, der Modellgröße, der Seed-Zielgruppengröße und der Schaltfläche „Senden“.](/help/assets/collaborate/expand/expansion-audience-detail.png){zoomable="yes"}

In dieser Ansicht haben Sie folgende Möglichkeiten:

* Namen der Erweiterungszielgruppe bearbeiten
* Erstellungsdatum und -uhrzeit anzeigen
* Vergleichen der Größe der Seed-Zielgruppe mit der generierten Größe der Erweiterungszielgruppe
* Überprüfen Sie den Übereinstimmungsschlüssel, der zum Generieren der Zielgruppe verwendet wird

Wenn Sie bereit sind, wählen Sie **[!UICONTROL An Partner senden]** aus, um die Erweiterungszielgruppe an Ihren Mitarbeiter zu senden. Die Zielgruppe verbleibt im **[!UICONTROL Entwurf]**-Status, bis Sie sie senden, und wird dann in **[!UICONTROL Aktiv]** aktualisiert.

>[!NOTE]
>
>Wenn für Ihren Mitarbeiter kein Ziel konfiguriert ist, ist **[!UICONTROL An Partner senden]** nicht verfügbar. In einer Meldung wird erläutert, dass Ihr Mitarbeiter zuerst ein Ziel einrichten muss.

>[!IMPORTANT]
>
>Eine Erweiterungszielgruppe läuft 7 Tage nach ihrer Generierung ab, wenn sie nicht an Ihren Mitarbeiter gesendet wird.

## Eine Erweiterungszielgruppe empfangen und aktivieren {#receive-activate-expansion-audience}

Wenn Sie eine Erweiterungszielgruppe senden, stellt Collaboration diese entsprechend der für die Verbindung konfigurierten Aktivierungseinstellung für Ihren Mitarbeiter bereit:

* Wenn **Automatische Aktivierung** aktiviert ist, aktiviert Collaboration die Erweiterungszielgruppe automatisch für das konfigurierte Ziel Ihres Mitarbeiters und wird auf seiner Registerkarte [Aktivieren](./activate.md#activated-audiences) angezeigt.
<!-- Beta release: automatic activation is the only available activation setting. Uncomment the manual activation guidance below when manual activation is introduced with the GA release. -->
<!-- * If **manual activation** is enabled, the expansion audience appears in your collaborator's [Received audiences](./activate.md#received-audiences) section of the **[!UICONTROL Activate]** tab, and your collaborator must manually activate it. -->

## Nächste Schritte

Nachdem Sie die Erweiterungszielgruppe gesendet haben, verwenden Sie die Registerkarte [Entdecken](./discover.md), um sie mit anderen Zielgruppen zu vergleichen, oder die Registerkarte [Aktivieren](./activate.md), um ihre Aktivierung nachzuverfolgen.
