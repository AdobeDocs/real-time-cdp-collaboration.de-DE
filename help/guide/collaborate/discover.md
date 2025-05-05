---
title: Überschneidungen erkennen und Zielgruppen vergleichen
description: Entdecken Sie Überschneidungen zwischen Ihren Zielgruppen und denen Ihrer Mitwirkenden. Erfahren Sie, wie Sie die besten Audiences für die Verwendung in Ihren Kampagnen ermitteln.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 24%

---

# Überschneidungen erkennen und Zielgruppen vergleichen

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>Der **[!UICONTROL Entdecken]**-Arbeitsbereich ist nur verfügbar, wenn der Anwendungsfall **Zielgruppenerkennung** während [ Verbindungsprozesses aktiviert ](../connect/establishing-connections.md#connection-settings). Weitere Informationen zu Anwendungsfällen finden Sie im Handbuch [Verwalten von ](./manage-projects.md#project-use-cases)&quot;.

Nachdem Sie [Projekt erstellt](/help/guide/collaborate/manage-projects.md) innerhalb eines Kooperationsbereichs zwischen einem Advertiser und einem Publisher erstellt haben, können Sie jetzt Ihre Zielgruppen mit den Zielgruppen Ihres Mitarbeiters vergleichen. Auf diese Weise können Sie Überschneidungen zwischen Zielgruppen erkennen und Einblicke erhalten, die nach Übereinstimmungsschlüsseln oder Identitäten aufgeschlüsselt sind. Dies hilft Advertisern bei der Entscheidung, welche Zielgruppen für die Aktivierung mit Publishern freigegeben werden sollen.

>[!IMPORTANT]
>
>Alle [Datenskizzen](/help/guide/glossary.md#sketches) die nicht aktualisiert oder aktualisiert wurden, werden nach 7 Tagen gelöscht. In diesem Fall werden die Zahlen, die in den verschiedenen Überschneidungsberichten auf dieser Seite angezeigt werden, auf null gesetzt, und die Freigabe einer Zielgruppe ist für diese abgelaufenen Zielgruppen nicht mehr verfügbar. Datenskizzen werden automatisch für Zielgruppen mit einem [aktiven Aktualisierungszeitplan](/help/guide/setup/onboard-audiences.md#schedule) aktualisiert.

![Entdecken Sie Überschneidungen](/help/assets/collaborate/discover-overlaps/discover-overlaps.png)

Die Übereinstimmungsschlüssel, die zum Erkennen und Vergleichen von Zielgruppen verwendet werden, werden festgelegt, wenn Sie [eine Verbindung mit einem Herausgeber herstellen](/help/guide/connect/establishing-connections.md#connection-settings). Um die in Vorbereitung auf die Ausführung von Kampagnen angegebenen Überschneidungsprozentsätze zu ändern, können Sie Übereinstimmungsschlüssel entfernen, aber an dieser Stelle keine neuen Übereinstimmungsschlüssel hinzufügen. Gehen Sie dazu zu den [Verbindungseinstellungen](/help/guide/connect/establishing-connections.md#connection-settings) zwischen den Mitarbeitern.

![Bildschirm „Übereinstimmungsschlüssel bearbeiten“](/help/assets/collaborate/discover-overlaps/edit-match-keys.png)

## Voraussetzungen {#prerequisites}

Um die Funktion auf der Registerkarte **[!UICONTROL Entdecken]** des Workflows **[!UICONTROL Zusammenarbeiten]** in vollem Umfang zu nutzen, haben Sie bereits:

* [Importierte Zielgruppen](/help/guide/setup/onboard-audiences.md)
* [Verbunden](/help/guide/connect/establishing-connections.md) mit einem gewünschten Advertiser oder Publisher, wobei der Anwendungsfall **Zielgruppenerkennung** aktiviert ist
* [hat ein Projekt erstellt](/help/guide/collaborate/manage-projects.md) zwischen Ihnen und einem Mitarbeiter

Sobald die oben genannten Voraussetzungen erfüllt sind, können Sie die Überschneidung zwischen Ihren Zielgruppen und denen Ihrer Mitarbeiter untersuchen und vergleichen.

## Vergleichen von Zielgruppen {#compare-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_compare_audiences"
>title="Vergleichen von Zielgruppen"
>abstract="Entdecken Sie Überschneidungen zwischen Ihren Zielgruppen und den Zielgruppen Ihrer oder Ihres Mitwirkenden. Sie können die Einstellungen in der Dropdown-Auswahl anpassen, um Überschneidungen zwischen einer oder mehreren Ihrer Zielgruppen mit einer oder mehreren der Zielgruppen Ihrer oder Ihres Mitwirkenden zu ermitteln."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_your_identity_count"
>title="Ihre Identitätsanzahl"
>abstract="Die Anzahl der Profile mit dieser ausgewählten Identität, die Teil Ihrer ausgewählten Zielgruppe sind"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_collaborator_identity_count"
>title="Identitätsanzahl von Mitwirkenden"
>abstract="Die Anzahl der Profile mit dieser ausgewählten Identität, die Teil der ausgewählten Zielgruppe Ihrer oder Ihres Mitwirkenden sind"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_count"
>title="Anzahl sich überschneidender Identitäten"
>abstract="Die Anzahl der Profile mit dieser ausgewählten Identität, die sowohl in Ihrer Zielgruppe als auch in der Zielgruppe Ihrer oder Ihres Mitwirkenden vorhanden sind"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_percentage"
>title="Prozentsatz sich überschneidender Identitäten"
>abstract="Der Prozentsatz der Profile, die sich zwischen Ihrer ausgewählten Zielgruppe und der ausgewählten Zielgruppe Ihrer oder Ihres Mitwirkenden überschneiden."

Mit der Karte „Zielgruppen vergleichen“ erhalten Sie ausführliche Informationen über die Überschneidung zwischen Ihren und den Zielgruppen Ihrer Mitarbeiter. Sie können auswählen, ob Sie eine der folgenden Zielgruppenkombinationen vergleichen möchten:

* Eine Ihrer Zielgruppen gegen eine der Zielgruppen Ihres Mitarbeiters
* Eine Ihrer Zielgruppen gegen alle Zielgruppen Ihres Mitarbeiters
* Alle Zielgruppen für eine der Zielgruppen Ihres Mitarbeiters
* Alle Ihre Zielgruppen im Vergleich zu allen Zielgruppen Ihres Mitarbeiters

Die angezeigten Informationen beziehen sich auf:

| Metrik | Beschreibung |
|---------|----------|
| **[!UICONTROL Anzahl der Identitäten]** (Ihres) | Die Anzahl der Profile mit einer ausgewählten Identität, die Teil Ihrer ausgewählten Zielgruppe sind. |
| **[!UICONTROL Anzahl der Identitäten]** (Ihr Mitarbeiter) | Die Anzahl der Profile mit einer ausgewählten Identität, die Teil der ausgewählten Zielgruppe Ihres Mitarbeiters sind. |
| **[!UICONTROL Identitäten überschneiden sich]** | Die Anzahl der Profile mit einer ausgewählten Identität, die sowohl in Ihrer Audience als auch in der Audience Ihres Mitarbeiters vorhanden sind. |
| **[!UICONTROL Überschneidungsprozentsatz]** | Der Prozentsatz der Profile, die sich zwischen Ihrer ausgewählten Zielgruppe und der ausgewählten Zielgruppe Ihrer oder Ihres Mitwirkenden überschneiden. |
| **[!UICONTROL Aufschlüsselung der Identitäten nach Übereinstimmungsschlüssel]** | Zeigen Sie basierend auf den Übereinstimmungsschlüsseln, die Sie und Ihr Mitarbeiter für das Projekt vereinbart haben, die Komposition der Identitäten in den Überschneidungsberechnungen nach individuellen Übereinstimmungsschlüsseln an. |

{style="table-layout:auto"}

>[!TIP]
>
>Der Überschneidungsprozentsatz ist möglicherweise nicht immer für alle Zielgruppen verfügbar. Die Sichtbarkeit des Indikators für den Überschneidungsprozentsatz hängt von der Einstellung ab, die Ihr Mitarbeiter für eine Zielgruppe im Abschnitt [Metadatensichtbarkeit“ ausgewählt ](/help/guide/setup/onboard-audiences.md#metadata-visibility).

## Relevante Zielgruppen {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="Relevante Zielgruppen"
>abstract="Basierend auf den Prozentsätzen für die Überschneidungen könnten diese Publisher-Zielgruppen gut zu Ihrer Kampagne passen. <br><br> Die <b>Identitätsanzahl</b> ist die Zielgruppengröße des Publishers. <br><br> <b>Sich überschneidende Identitäten</b> stellt die Überschneidung zwischen der empfohlenen Publisher-Zielgruppe und allen Advertiser-Zielgruppen dar. <br><br> Die <b>Überschneidung in %</b> stellt die Anzahl der sich überschneidenden Identitäten dividiert durch die Größe <i>aller</i> Advertiser-Zielgruppen dar."

Die **[!UICONTROL Relevante Zielgruppen]** im Modul **[!UICONTROL Entdecken]** bietet eine kuratierte Liste der fünf häufigsten Zielgruppen basierend auf dem Überschneidungsprozentsatz. Mit dieser Funktion können Sie die Zielgruppen mit der höchsten Überschneidung mit Ihren aktuellen Daten schnell identifizieren, sodass Sie Ihre Kampagnen effektiver ansprechen können.

* **[!UICONTROL Identitätsanzahl]** ist die Zielgruppengröße des Herausgebers.
* **[!UICONTROL Überschneidende Identitäten]** stellt die Überschneidung zwischen der empfohlenen Publisher-Zielgruppe und allen Advertiser-Zielgruppen dar.
* **[!UICONTROL Überschneidung %]** steht für die Anzahl der sich überschneidenden Identitäten dividiert durch die Größe *aller* Advertiser-Zielgruppen.

![Ansicht „Relevante Zielgruppen“](/help/assets/collaborate/discover-overlaps/relevant-audiences-highlighted.png)

## Entdecken von Überschneidungen {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="Entdecken von Überschneidungen mit einzelnen Zielgruppen"
>abstract="Erhalten Sie Erkenntnisse bezüglich der Population dieser Zielgruppe und ihrer Überschneidungen mit der Gesamtheit der Identitäten der oder des Mitwirkenden."

![Entdecken Sie Überschneidungen mit verschiedenen Zielgruppenansichten](/help/assets/collaborate/discover-overlaps/discover-overlaps-cards-view.png)

Erhalten Sie ausführliche Informationen über die Zielgruppen Ihres Mitarbeiters und sehen Sie sich Überschneidungsinformationen an, indem Sie diese Zielgruppen entweder mit der Gesamtpopulation für alle Ihre Zielgruppen oder mit bestimmten Zielgruppen Ihres Mitarbeiters vergleichen.

>[!TIP]
>
>Einige der im Screenshot angegebenen Zahlen stehen möglicherweise nicht immer für alle Zielgruppen zur Verfügung. Ihre Sichtbarkeit hängt von der Einstellung ab, die Ihr Mitarbeiter für eine Zielgruppe im Abschnitt [Metadatensichtbarkeit“ ausgewählt ](/help/guide/setup/onboard-audiences.md#metadata-visibility).

## Nächste Schritte

Nachdem Sie die gewünschten Zielgruppen untersucht und entdeckt haben, können [ die Zielgruppen, ](/help/guide/collaborate/share.md) in den Kampagnen verwendet werden sollen, mit dem Herausgeber teilen.
