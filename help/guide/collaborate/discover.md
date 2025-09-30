---
title: Überschneidungen erkennen und Zielgruppen vergleichen
description: Entdecken Sie Überschneidungen zwischen Ihren Zielgruppen und denen Ihrer Mitwirkenden. Erfahren Sie, wie Sie die besten Audiences für die Verwendung in Ihren Kampagnen ermitteln.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: 3dd37dff0be104894cdfe42503b60056b25018e3
workflow-type: tm+mt
source-wordcount: '2069'
ht-degree: 17%

---

# Überschneidungen erkennen und Zielgruppen vergleichen

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>Der **[!UICONTROL Entdecken]**-Arbeitsbereich ist nur verfügbar, wenn der Anwendungsfall **Zielgruppenerkennung** während [ Verbindungsprozesses aktiviert ](../connect/establishing-connections.md#connection-settings). Weitere Informationen zu Anwendungsfällen finden Sie im Handbuch [Verwalten von ](./manage-projects.md#project-use-cases)&quot;.

Nach [Erstellen eines Projekts](/help/guide/collaborate/manage-projects.md) können Sie Ihre Zielgruppen mit Ihren Mitwirkenden vergleichen. Auf diese Weise können Sie relevante Zielgruppen für Kampagnen identifizieren und entscheiden, welche zur Aktivierung an Mitwirkende gesendet werden sollen.

>[!IMPORTANT]
>
>Alle [Datenskizzen](/help/guide/glossary.md#sketches) die nicht aktualisiert oder aktualisiert wurden, werden nach 7 Tagen gelöscht. In diesem Fall werden die Zahlen, die in den verschiedenen Überschneidungsberichten auf dieser Seite angezeigt werden, auf null gesetzt, und die Freigabe einer Zielgruppe ist für diese abgelaufenen Zielgruppen nicht mehr verfügbar. Datenskizzen werden automatisch für Zielgruppen mit einem [aktiven Aktualisierungszeitplan](/help/guide/setup/onboard-audiences.md#schedule) aktualisiert.

Die Übereinstimmungsschlüssel, die zum Erkennen und Vergleichen von Zielgruppen verwendet werden, werden [während des Verbindungsprozesses](/help/guide/connect/establishing-connections.md#connection-settings) eingerichtet. Übereinstimmungsschlüssel werden verwendet, um die Überschneidung zwischen Ihren Zielgruppen zu berechnen, und können ein- und ausgeschaltet werden. Um die Übereinstimmungsschlüssel zu bearbeiten, wählen Sie die Option **[!UICONTROL Übereinstimmungsschlüssel bearbeiten]** aus.

![Der Arbeitsbereich der Registerkarte „Entdecken“, auf dem die Einblicke zur Zielgruppe angezeigt werden.](/help/assets/collaborate/discover/discover-overview.png)

Das **[!UICONTROL Bearbeiten von Übereinstimmungsschlüsseln]** wird geöffnet, in dem Sie die Übereinstimmungsschlüssel, die Sie nicht verwenden möchten, deaktivieren können. Klicken Sie **[!UICONTROL Speichern]**, um Ihre Änderungen zu speichern.

![Das Dialogfeld „Übereinstimmungsschlüssel bearbeiten“ im Discover-Arbeitsbereich.](/help/assets/collaborate/discover/edit-match-keys.png)

## Voraussetzungen {#prerequisites}

Um die Registerkarte **[!UICONTROL Entdecken]** in Ihrem Projekt verwenden zu können, sollten Sie über Folgendes verfügen:

* [Sourced-Zielgruppen](/help/guide/setup/onboard-audiences.md) in Ihrem Konto
* [Verbunden](/help/guide/connect/establishing-connections.md) mit einem Mitarbeiter mit aktiviertem **Zielgruppenerkennung**-Anwendungsfall
* [hat ein Projekt erstellt](/help/guide/collaborate/manage-projects.md) zwischen Ihnen und einem Mitarbeiter

Sobald diese Voraussetzungen erfüllt sind, können Sie beginnen, Überschneidungen zwischen Ihnen und den Zielgruppen Ihrer Mitwirkenden zu untersuchen und zu vergleichen.

## Vergleichen von Zielgruppen {#compare-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_compare_audiences"
>title="Vergleichen von Zielgruppen"
>abstract="Entdecken Sie Überschneidungen zwischen Ihren Zielgruppen und den Zielgruppen Ihrer oder Ihres Mitwirkenden. Sie können die Einstellungen in der Dropdown-Auswahl anpassen, um Überschneidungen zwischen einer oder mehreren Ihrer Zielgruppen mit einer oder mehreren der Zielgruppen Ihrer oder Ihres Mitwirkenden zu ermitteln."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_your_identity_count"
>title="Ihre Identitätsanzahl"
>abstract="Die Anzahl der eindeutigen IDs innerhalb Ihrer ausgewählten Zielgruppe, basierend auf den Übereinstimmungsschlüsseln, die Sie und Ihre mitwirkende Person für das Projekt vereinbart haben."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_collaborator_identity_count"
>title="Identitätsanzahl von Mitwirkenden"
>abstract="Die Anzahl der eindeutigen IDs innerhalb der Zielgruppe Ihrer mitwirkenden Person, basierend auf den Übereinstimmungsschlüsseln, die Sie und die Person für das Projekt vereinbart haben."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_count"
>title="Anzahl sich überschneidender Identitäten"
>abstract="Die Anzahl der eindeutigen IDs, die sowohl in Ihren Zielgruppen als auch in denen Ihrer mitwirkenden Person vorhanden sind, basierend auf den Übereinstimmungsschlüsseln, die Sie und die Person für das Projekt vereinbart haben."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_percentage"
>title="Prozentsatz sich überschneidender Identitäten"
>abstract="Der Prozentsatz der Identitäten, die sich zwischen Ihrer ausgewählten Zielgruppe und der ausgewählten Zielgruppe Ihrer mitwirkenden Person überschneiden."

Im Abschnitt „Zielgruppen vergleichen“ erhalten Sie ausführliche Informationen über die Überschneidung zwischen Ihren und den Zielgruppen Ihrer Mitwirkenden. Um die Zielgruppenauswahl zu ändern, verwenden Sie die Dropdown-Auswahl oben im Abschnitt **[!UICONTROL Zielgruppen vergleichen]**. Sie können eine oder alle Zielgruppen Ihres Mitarbeiters und eine oder alle Zielgruppen Ihres Mitarbeiters auswählen, um sie miteinander zu vergleichen.

![Der Arbeitsbereich „Entdecken“ mit hervorgehobenem Zielgruppen-Selektor im Abschnitt „Zielgruppen vergleichen“.](/help/assets/collaborate/discover/compare-audiences-selector.png)

Im Abschnitt Vergleichen von Zielgruppen werden die folgenden Metriken angezeigt, die auf den Übereinstimmungsschlüsseln basieren, die Sie und Ihr Mitarbeiter für das Projekt vereinbart haben:

| Metrik | Beschreibung |
|---------|----------|
| **[!UICONTROL Anzahl der Identitäten]** (Ihres) | Die Anzahl der eindeutigen IDs innerhalb Ihrer ausgewählten Zielgruppe(n). |
| **[!UICONTROL Anzahl der Identitäten]** (Ihr Mitarbeiter) | Die Anzahl der eindeutigen IDs innerhalb der Zielgruppe(n) Ihres Mitarbeiters. |
| **[!UICONTROL Identitäten überschneiden sich]** | Die Anzahl der eindeutigen IDs, die sowohl in Ihren als auch in den Zielgruppen Ihres Mitarbeiters vorhanden sind. |
| **[!UICONTROL Überschneidung %]** | Der Prozentsatz der Profile, die sich zwischen Ihrer ausgewählten Zielgruppe und der ausgewählten Zielgruppe Ihrer oder Ihres Mitwirkenden überschneiden. |
| **[!UICONTROL Zielgruppenindex]** | Ein Score, der basierend auf der Anzahl und Überschneidung der zugrunde liegenden Zielgruppen angibt, wie stark sich eine Zielgruppe auf eine andere bezieht. Weitere Informationen zur Bedeutung der Bewertungen finden Sie im Abschnitt [Audience-Index](#audience-index-score). Die Zielgruppenindexwerte sind beim Vergleich mit der Grundlinie Ihres Mitarbeiters (alle Zielgruppen) nicht verfügbar. |
| **[!UICONTROL Aufschlüsselung der Identitäten nach Übereinstimmungsschlüssel]** | Die Aufschlüsselung der Identitäten, die für jeden im Projekt ausgewählten Übereinstimmungsschlüssel übereinstimmen, basierend auf den für jeden Mitarbeiter ausgewählten Zielgruppen. |

{style="table-layout:auto"}

>[!NOTE]
>
>Die Prozentzahl der Überschneidung und der Zielgruppenindex-Wert sind möglicherweise nicht immer für alle Zielgruppen verfügbar. Die Sichtbarkeit des Überschneidungsprozentsatzes und des Zielgruppenindex-Scores hängt von der Einstellung ab, die Ihr Mitarbeiter für eine Zielgruppe im Abschnitt [Metadatensichtbarkeit“ ausgewählt ](/help/guide/setup/onboard-audiences.md#metadata-visibility).

Wenn Ihr Mitarbeiter weder den Zielgruppenindex noch den Überschneidungsprozentsatz aktiviert hat, sind für die Zielgruppe keine Vergleichsdaten verfügbar.

## Relevante Zielgruppen {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="Relevante Zielgruppen"
>abstract="Basierend auf den Prozentsätzen der Überschneidungen könnten diese Zielgruppen gut zu Ihrer Kampagne passen. <br><br> Die <b>Anzahl der Identitäten</b> ist die Größe der Zielgruppe der bzw. des Mitwirkenden. <br><br> <b>Überlappende Identitäten</b> stellt die Überschneidung zwischen der empfohlenen Zielgruppe und allen Ihren Zielgruppen dar. <br><br><b>Überschneidung %</b> stellt die Anzahl der sich überschneidenden Identitäten geteilt durch die Größe <i>aller</i> Ihrer Zielgruppen dar."

Der Abschnitt **[!UICONTROL Relevante Zielgruppen]** auf der Registerkarte **[!UICONTROL Entdecken]** enthält eine kuratierte Liste der fünf häufigsten Zielgruppen, basierend auf dem Prozentsatz der Überschneidung zwischen der Zielgruppe Ihres Mitarbeiters und allen Ihren Zielgruppen. Mit dieser Funktion können Sie die Zielgruppen mit der höchsten Überschneidung schnell identifizieren, sodass Sie Ihre Kampagnen effektiver ansprechen können. Wechseln Sie mithilfe der Seitenauswahl oben rechts im Abschnitt zwischen den relevanten Zielgruppen.

![Der Arbeitsbereich „Entdecken“ mit hervorgehobenem Abschnitt „Relevante Zielgruppen“.](/help/assets/collaborate/discover/relevant-audiences.png)

>[!NOTE]
>
>Die Sichtbarkeit der Zielgruppen Ihres Mitarbeiters hängt von der Einstellung ab, die Ihr Mitarbeiter für eine Zielgruppe im Abschnitt [Verbindungszugriff](/help/guide/setup/onboard-audiences.md#connection-access) und im Abschnitt [Metadatensichtbarkeit](/help/guide/setup/onboard-audiences.md#metadata-visibility) ausgewählt hat. Wenn Ihr Mitarbeiter alle Zielgruppen auf „privat“ gesetzt hat, werden in diesem Abschnitt keine Zielgruppen angezeigt.

Im Abschnitt **[!UICONTROL Relevante Zielgruppen]** werden die folgenden Informationen für jede empfohlene Zielgruppe angezeigt:

| Metrik | Beschreibung |
|---------|----------|
| **[!UICONTROL Anzahl der Identitäten]** | Die Anzahl der eindeutigen IDs innerhalb der Zielgruppe. |
| **[!UICONTROL Identitäten überschneiden sich]** | Die Anzahl der eindeutigen IDs, die sich zwischen der empfohlenen Zielgruppe und allen Ihren Zielgruppen überschneiden. |
| **[!UICONTROL Überschneidung %]** | Der Prozentsatz der Identitäten mit Überschneidungen zwischen der empfohlenen Zielgruppe und allen Ihren Zielgruppen. |
| **[!UICONTROL Zielgruppenindex]** | Ein Score, der basierend auf der Anzahl und Überschneidung der zugrunde liegenden Zielgruppen angibt, wie stark sich eine Zielgruppe auf eine andere bezieht. Weitere Informationen zur Bedeutung der Bewertungen finden Sie im Abschnitt [Audience-Index](#audience-index-score). |
| **[!UICONTROL Zielgruppenkategorien]** | Die Kategorien, die Ihr Mitarbeiter der Zielgruppe zugewiesen hat. |
| **[!UICONTROL Übereinstimmungsschlüssel]** | Die Übereinstimmungsschlüssel, die Ihr Mitarbeiter für die Zielgruppe ausgewählt hat. |

{style="table-layout:auto"}

Wenn der Zielgruppenindex-Score für eine der Zielgruppen Ihres Mitarbeiters aktiviert ist, basieren die relevanten Zielgruppen auf dem Zielgruppenindex-Score, und Zielgruppen, für die der Zielgruppenindex nicht aktiviert wurde, werden nicht einbezogen. Relevante Zielgruppen basierend auf dem Audience-Index-Score werden so sortiert, dass zuerst der höchste Index-Score angezeigt wird. Wenn der Zielgruppenindex für keine der Zielgruppen Ihres Mitarbeiters aktiviert ist, basieren die relevanten Zielgruppen auf dem Überschneidungsprozentsatz.

## Entdecken von Überschneidungen {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="Entdecken von Überschneidungen mit einzelnen Zielgruppen"
>abstract="Gewinnen Sie Erkenntnisse zu Überschneidungen zwischen Ihren Zielgruppen und den Zielgruppen Ihrer mitwirkenden Person."

Entdecken Sie Überschneidungen, um Einblicke in den Vergleich Ihrer Zielgruppen mit den Zielgruppen Ihrer Mitwirkenden zu erhalten. In diesem Abschnitt werden standardmäßig alle Zielgruppen Ihrer Mitarbeiter mit den Zielgruppen Ihrer Mitarbeiter verglichen. Verwenden Sie das Paginierungssteuerelement am unteren Rand des Abschnitts, um durch die verfügbaren Zielgruppen zu navigieren.

![Der Arbeitsbereich „Entdecken“ mit hervorgehobenem Abschnitt „Entdecken überschneidet“.](/help/assets/collaborate/discover/discover-overlaps.png)

>[!NOTE]
>
>Die Sichtbarkeit der Zielgruppen Ihres Mitarbeiters hängt von der Einstellung ab, die Ihr Mitarbeiter für eine Zielgruppe im Abschnitt [Verbindungszugriff](/help/guide/setup/onboard-audiences.md#connection-access) und im Abschnitt [Metadatensichtbarkeit](/help/guide/setup/onboard-audiences.md#metadata-visibility) ausgewählt hat. Wenn Ihr Mitarbeiter alle Zielgruppen auf „privat“ gesetzt hat, werden in diesem Abschnitt keine Zielgruppen angezeigt.

Wenn Ihr Mitarbeiter weder den Zielgruppenindex noch den Überschneidungsprozentsatz aktiviert hat, wird die Zielgruppe nicht angezeigt.

Um Ihre Zielgruppenauswahl zu ändern, wählen Sie **[!UICONTROL Zielgruppe ändern]** aus.

![Der Arbeitsbereich „Entdecken“ mit hervorgehobener Option „Zielgruppe ändern“.](/help/assets/collaborate/discover/change-audience.png)

Das Dialogfeld **[!UICONTROL Zielgruppe ändern]** wird geöffnet, in dem Sie eine bestimmte Zielgruppe auswählen können, die mit den Zielgruppen Ihres Mitarbeiters verglichen werden soll. Wählen Sie die gewünschten Zielgruppen aus, oder löschen Sie Ihre Auswahl, um alle Zielgruppen auszuwählen, und klicken Sie dann auf **[!UICONTROL Speichern]**.

![Das Dialogfeld „Zielgruppe ändern“ im Discover-Arbeitsbereich.](/help/assets/collaborate/discover/change-audience-selection.png)

Nach Auswahl der gewünschten Zielgruppen werden im Abschnitt **[!UICONTROL Überschneidungen erkennen]** die folgenden Informationen zu jeder Zielgruppe angezeigt:

| Metrik | Beschreibung |
|---------|----------|
| **[!UICONTROL Anzahl der Identitäten]** | Die Anzahl der eindeutigen IDs innerhalb der Zielgruppe. |
| **[!UICONTROL Identitäten überschneiden sich]** | Die Anzahl der eindeutigen IDs, die sich zwischen der empfohlenen Zielgruppe und allen Ihren Zielgruppen überschneiden. |
| **[!UICONTROL Überschneidung %]** | Der Prozentsatz der Identitäten mit Überschneidungen zwischen der empfohlenen Zielgruppe und allen Ihren Zielgruppen. |
| **[!UICONTROL Zielgruppenindex]** | Ein Score, der basierend auf der Anzahl und Überschneidung der zugrunde liegenden Zielgruppen angibt, wie stark sich eine Zielgruppe auf eine andere bezieht. Weitere Informationen zur Bedeutung der Bewertungen finden Sie im Abschnitt [Audience-Index](#audience-index-score). |
| **[!UICONTROL Zielgruppenkategorien]** | Die Kategorien, die Ihr Mitarbeiter der Zielgruppe zugewiesen hat. |
| **[!UICONTROL Übereinstimmungsschlüssel]** | Die Übereinstimmungsschlüssel, die Ihr Mitarbeiter für die Zielgruppe ausgewählt hat. |

{style="table-layout:auto"}

## Zielgruppenindexwert {#audience-index-score}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_audience_index_score"
>title="Zielgruppenindexwert"
>abstract="Zielgruppenindexwerte sind eine differenzierte Metrik, die anhand der zugrunde liegenden Anzahl und Überschneidungen der Zielgruppen anzeigt, wie stark eine Zielgruppe mit einer anderen in Beziehung steht. Der Rohindexwert wird in Relevanzbereiche übertragen, die die Zielgruppenindexwerte von sehr niedrig bis sehr hoch kategorisieren. Auf diese Weise können Sie die Stärke der Beziehung zwischen Ihrer Zielgruppe und der Zielgruppe der mitwirkenden Person schnell bewerten."

Zielgruppenindexwerte sind eine differenzierte Metrik, die anhand der zugrunde liegenden Anzahl und Überschneidungen der Zielgruppen anzeigt, wie stark eine Zielgruppe mit einer anderen in Beziehung steht. Auf diese Weise können Sie Zielgruppeneinblicke kontextualisieren und Zielgruppen mit hohem Potenzial für Interessenten- und Kampagnen-Targeting identifizieren.

Der Index-Score wird anhand der folgenden Formel berechnet:

![Die Formel zur Berechnung der Indexbewertung.](/help/assets/collaborate/discover/index-score-formula.png)

Stellen Sie sich vor, ein Automobilhersteller möchte eine Werbekampagne mit einem großen Fernsehverlag für ein neues SUV-Modell durchführen. Der Fahrzeughersteller hat Daten darüber, wem derzeit ein ähnliches Modell gehört und möchte dieses verwenden, um zusätzliche potenzielle Kunden zu finden, die es in Kunden umwandeln könnten. Der Automobilhersteller betrachtet die Zielgruppen des CTV-Verlags, um eine relevante Zielgruppe zu finden, die den aktuellen SUV-Besitzern sehr nahe kommt.

![Der Autowerber im Vergleich zum Publikum des CTV-Verlags.](/help/assets/collaborate/discover/audience-index-score-example.png)

Die Indexwerte werden berechnet und können verwendet werden, um den wahrscheinlichen Erfolg der Kampagne zu bestimmen:

| CTV Publisher-Zielgruppe | Formel | Index-Bewertung (i) | Interpretation |
|------------------------|-------------|----------------|----------------|
| Baseline (alle Zielgruppen) | ((1,3 M / 1,3 M) / (50 M / 50 M)) * 100 | 100 | Dies dient als Grundlinie, mit der die anderen Zielgruppen Ihres Mitarbeiters verglichen werden. |
| Binge Watchers | ((500 K / 1,3 M) / (20 M / 50 M)) * 100 | 96 | Wenn Sie diese Zielgruppe ansprechen, ist die Wahrscheinlichkeit, SUV-Besitzer zu erreichen, im Vergleich zur Grundlinie um 4 % geringer. |
| Comedy-Liebhaber | ((200 K / 1,3 M) / (6 M / 50 M)) * 100 | 128 | Wenn Sie diese Zielgruppe ansprechen, erreichen Sie mit 28 % höherer Wahrscheinlichkeit SUV-Besitzer im Vergleich zur Baseline. |
| Männer 25-34 | ((700 K / 1,3 M) / (12 M / 50 M)) * 100 | 224 | Wenn Sie diese Zielgruppe ansprechen, erreichen Sie mit 124 % höherer Wahrscheinlichkeit SUV-Besitzer im Vergleich zur Grundlinie. |
| Technikbegeisterte | ((500 K / 1,3 M) / (8 M / 50 M)) * 100 | 240 | Wenn Sie diese Zielgruppe ansprechen, erreichen Sie mit 140 % höherer Wahrscheinlichkeit SUV-Besitzer im Vergleich zur Grundlinie. |

{style="table-layout:auto"}

Um besser verstehen zu können, wie sich die Indexbewertungen auf Ihre Kampagne auswirken, werden Relevanzbänder zusammen mit den Bewertungen bereitgestellt.

### Relevanzbereiche {#audience-index-relevance-bands}

Um einen einfachen Vergleich über verschiedene Zielgruppen und Kampagnen hinweg zu ermöglichen, übersetzt Collaboration die Indexwerte in Relevanzbänder (sehr niedrig bis sehr hoch). Auf diese Weise können Sie die Stärke der Beziehung zwischen Ihrer Zielgruppe und der Zielgruppe der mitwirkenden Person schnell bewerten.

| Index-Bewertung (i) | Relevanzbereich | Beschreibung |
|---------------|----------|-----------|
| i &lt; 60 | Sehr niedrig | Die Überschneidung ist bei der Zielgruppe im Vergleich zu Ihrer Zielgruppe viel geringer, was auf eine sehr schwache Beziehung hinweist. Kunden, die diese Zielgruppe verwenden, erreichen ihre Zielgruppe mit deutlich geringerer Wahrscheinlichkeit. |
| 60 &lt; i &lt; 80 | Niedrig | Die Überschneidung ist bei der Zielgruppe im Vergleich zu Ihrer Zielgruppe etwas geringer, was auf eine schwache Beziehung hindeutet. Kunden, die diese Zielgruppe verwenden, erreichen ihre Zielgruppe mit geringerer Wahrscheinlichkeit. |
| 80 &lt; i &lt; 120 | Mittel | Die Überschneidung ist in der Zielgruppe genauso verbreitet wie in Ihrer Zielgruppe, was auf eine typische Beziehung hinweist. Kunden, die diese Zielgruppe verwenden, haben eine durchschnittliche Wahrscheinlichkeit, ihre Zielgruppe zu erreichen. |
| 120 &lt; i &lt; 140 | Hoch | Die Überschneidung ist bei der Zielgruppe häufiger als bei Ihrer Zielgruppe und zeigt eine starke Beziehung. Kunden, die diese Zielgruppe verwenden, erreichen mit höherer Wahrscheinlichkeit ihre Zielgruppe. |
| I > 140 | Sehr hoch | Die Überschneidung ist bei der Zielgruppe im Vergleich zu Ihrer Zielgruppe viel häufiger, was eine sehr starke Beziehung widerspiegelt. Kunden, die diese Zielgruppe verwenden, erreichen ihre Zielgruppe mit viel höherer Wahrscheinlichkeit. |

{style="table-layout:auto"}

Innerhalb des Abschnitts „Überschneidungen erkennen“ zeigt der Zielgruppenindex-Score die Relevanzspanne neben dem Score an. Der Score wird farbcodiert, um das Relevanzband anzugeben, sodass die Stärke der Beziehung auf einen Blick leicht erkannt werden kann. Sehr niedere und niedere Relevanzbänder werden in orangefarbenen, mittlere Relevanzbänder in Schwarz und Bänder mit hoher und sehr hoher Relevanz in Grün angezeigt.

## Nächste Schritte

Nachdem Sie die gewünschten Zielgruppen untersucht und entdeckt haben, können [ die Zielgruppen ](/help/guide/collaborate/activate.md), die in den Kampagnen verwendet werden sollen.
