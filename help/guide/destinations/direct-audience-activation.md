---
title: Zielgruppen direkt aktivieren (1P Audience Activation) - Beta
description: Erfahren Sie, wie Sie Ihre eigenen oder freigegebenen Erstanbieter-Zielgruppen ohne Projekt aktivieren, ein Ziel auswählen, Feldzuordnungen überprüfen und einen Aktivierungsplan festlegen.
badgeBeta: label="Beta" type="Informative"
source-git-commit: 5f823194a18468b9205f64853551719ae8a3752f
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 1%
---

# Zielgruppen direkt aktivieren (1P Audience Activation) {#activate-audiences-directly}

Verwenden Sie die direkte Erstanbieter-Zielgruppenaktivierung (1P), [!DNL Adobe Real-Time CDP Collaboration] Zielgruppen an ein Ziel zu senden, ohne ein Projekt zu erstellen. Aktivieren Sie Zielgruppen, deren Inhaber Sie sind, oder freigegebene Zielgruppen für die Erstanbieter-Nutzung.

Beginnen Sie mit einem konfigurierten Ziel oder **[!UICONTROL Aktivierte Zielgruppen]** wählen Sie dann Zielgruppen aus und legen Sie den Aktivierungsplan fest.

Informationen zum Senden und Aktivieren von Zielgruppen über ein Kooperationsprojekt finden Sie unter [Senden und Aktivieren von Zielgruppen in einem Projekt](/help/guide/collaborate/activate.md).

## Zielgruppenzugriff für die Aktivierung {#audience-access-for-activation}

Überprüfen Sie die Zielgruppenquelle, um festzustellen, ob Sie vor der Aktivierung eine Finanzhilfe benötigen.

| Zielgruppenquelle | Zugangsvoraussetzung |
| --- | --- |
| Eigene Zielgruppen | Sie besitzen die Zielgruppen. |
| Für Sie freigegebene Zielgruppen | Sie benötigen eine aktive Genehmigung mit direkter Aktivierungsberechtigung. Der Anbieter behält das Eigentum. |

{style="table-layout:auto"}

Mit einer virtuellen Zielgruppe erhalten Sie Zugriff auf eine freigegebene Zielgruppe per Verweis, ohne die Daten zu verschieben. Anschließend können Sie die Zielgruppe aktivieren, um ihre Daten an Ihr ausgewähltes Ziel zu senden.

Weitere Informationen zu Grants und Anbietersteuerelementen finden Sie unter [Zugriff auf virtuelle Zielgruppen (Zielgruppenzuweisungen)](/help/guide/setup/virtual-audience-access.md).

## Voraussetzungen {#prerequisites}

Bevor Sie beginnen, bestätigen Sie, dass Sie Folgendes haben:

* Eine Zielgruppe, deren Inhaber Sie sind oder die über einen qualifizierten Erstanbieter-Zuschuss (1P) freigegeben wurde.
* Ein konfiguriertes Ziel, das Sie steuern und das die direkte Aktivierung unterstützt.
* Mindestens eine Zuordnung eines Übereinstimmungsschlüssels für das Ziel.

Um eine freigegebene Zielgruppe zu aktivieren, bestätigen Sie, dass ihre aktive, für eine Verbindung geltende Gewährung die [Eignungsbedingungen](#check-shared-audience-access) erfüllt. Verwenden Sie den **[!UICONTROL Aktivierung]** Arbeitsbereich. Sie benötigen kein Projekt.

### Berechtigung für freigegebene Zielgruppen {#check-shared-audience-access}

Der Zuschuss muss jede Bedingung erfüllen, um die direkte Aktivierung zu unterstützen.

| Anforderung | Bedingung |
| --- | --- |
| Zielgruppen-Berechtigung | Die Gewährung umfasst die Berechtigung zur direkten Aktivierung. |
| Zugriffsdauer | Die Gewährung ist entweder auf unbestimmte Zeit oder innerhalb des angegebenen Datumsbereichs aktiv. |

{style="table-layout:auto"}

Mit der separaten Berechtigung **[!UICONTROL Neue Zielgruppe erstellen]** können Sie eine freigegebene Zielgruppe für die Erstellung von Kohorten-Zielgruppen verwenden. Diese Berechtigung ist für die direkte Aktivierung nicht erforderlich.

### Zielfeldzuordnungen {#review-destination-field-mappings}

Die direkte Aktivierung verwendet die für Ihr Ziel konfigurierten Übereinstimmungsschlüssel-Zuordnungen. Bei der Aktivierung werden keine Übereinstimmungsschlüssel ausgewählt.

Informationen zum Konfigurieren von Zielen finden Sie unter [Ziele - Übersicht](../destinations/overview.md).

## Direkte Aktivierung starten {#start-direct-activation}

Beginnen Sie mit einem konfigurierten Ziel oder der Liste der aktivierten Zielgruppen. Adobe Experience Platform-Ziele unterstützen keine First-Party-Aktivierung.

### Von einem Ziel starten {#start-from-a-destination}

Um den Workflow mit einem ausgewählten Ziel zu öffnen, starten Sie mit diesem konfigurierten Ziel. Öffnen Sie zunächst den Arbeitsbereich **[!UICONTROL Aktivierung]** und wählen Sie &quot;**[!UICONTROL &quot;]**.

Wählen Sie als Nächstes **[!UICONTROL Zielgruppen aktivieren]** aus den Aktionen für das Ziel aus, das Sie verwenden möchten.

Der Workflow wird mit dem ausgewählten Ziel geöffnet. Fahren Sie dann mit [Konfigurieren der Aktivierung](#configure-the-activation) fort.

### Von aktivierten Zielgruppen starten {#start-from-activated-audiences}

Um ein Ziel im Workflow auszuwählen, starten Sie in der Liste der aktivierten Zielgruppen. Öffnen Sie zunächst den Arbeitsbereich **[!UICONTROL Aktivierung]** und wählen Sie **[!UICONTROL Aktivierte Zielgruppen]**.

Starten Sie den Workflow als Nächstes, indem Sie **[!UICONTROL Zielgruppe aktivieren]** auf der Seite auswählen oder das Symbol Hinzufügen auswählen (![Zielgruppenaktivierung hinzufügen.](/help/assets/icons/plus.png)) und dann &quot;**[!UICONTROL aktivieren]**.

Der Workflow wird geöffnet, ohne dass ein Ziel ausgewählt ist. Fahren Sie dann mit [Konfigurieren der Aktivierung](#configure-the-activation) fort.

## Konfigurieren der Aktivierung {#configure-the-activation}

Wählen Sie pro Aktivierung eine Zielgruppe aus Ihren eigenen Zielgruppen oder aus den für Sie freigegebenen Zielgruppen aus. Verwenden Sie das vorausgewählte Ziel oder wählen Sie ein konfiguriertes Ziel aus, wenn keines ausgewählt ist. Der Workflow wendet die [vorhandenen Zuordnungen](#review-destination-field-mappings) an, die für dieses Ziel konfiguriert sind.

Wählen Sie aus, wann die Aktivierung ausgeführt werden soll, und überprüfen Sie dann die ausgewählte Zielgruppe, das ausgewählte Ziel und den ausgewählten Zeitplan, bevor Sie den Bericht übermitteln.

## Zugreifen auf Änderungen und geplante Ausführungen {#access-changes-and-scheduled-runs}

Aktivieren Sie eine freigegebene Zielgruppe nur, solange der Anbieter Zugriff gewährt.

| Zugriffsänderung | Ergebnis |
| --- | --- |
| Der Zuschuss läuft aus | Das System verarbeitet den Ablauf stündlich. Der Empfänger verliert den Zugriff auf die virtuelle Zielgruppe, nachdem der Ablauf verarbeitet wurde. |
| Der Anbieter widerruft die Gewährung | Der Empfänger verliert sofort den Zugriff auf die virtuelle Zielgruppe. |
| Eine geplante Aktivierung wird ausgeführt | Das System prüft den Zuschuss. Zielgruppen mit widerrufenen oder abgelaufenen Zuschüssen sind nicht für die Aktivierung geeignet. |

{style="table-layout:auto"}

Ablauf oder Sperrung entfernt keine Zielgruppendaten, die bereits an ein Ziel gesendet wurden.

## Nächste Schritte {#next-steps}

Nachdem Sie Zielgruppen aktiviert haben, verwenden Sie diese Handbücher zum Verwalten von Zielen oder Collaborator-Verbindungen.

* [Konfigurieren und Verwalten von Zielen](/help/guide/destinations/manage-destinations.md)
* [Verwalten von Collaborator-Verbindungen](/help/guide/connect/manage-connections.md)
