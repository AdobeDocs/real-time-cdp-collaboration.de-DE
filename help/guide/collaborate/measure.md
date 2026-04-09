---
title: Leistung messen
description: Messen Sie die Leistung Ihrer Kampagnen über verschiedene Kanäle hinweg. Erfahren Sie, wie Sie verschiedene Berichte verwenden und interpretieren.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
source-git-commit: 0cf888e36ffc4730fc8de4d8adccae0e0fc2caa8
workflow-type: tm+mt
source-wordcount: '1949'
ht-degree: 6%

---

# Leistung messen

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>Der **[!UICONTROL Measure]**-Arbeitsbereich ist nur verfügbar, wenn der **Measurement**-Anwendungsfall [während des Verbindungsprozesses) &#x200B;](../connect/establishing-connections.md#connection-settings) wurde. Weitere Informationen zu Anwendungsfällen finden Sie im Handbuch [Verwalten von &#x200B;](./manage-projects.md#project-use-cases)&quot;.

Erfahren Sie mehr über die verfügbaren Berichte in Adobe Real-Time CDP Collaboration und lernen Sie, wie Sie die Leistung Ihrer Marketing-Kampagnen kanalübergreifend messen und analysieren können.

## Voraussetzungen {#prerequisites}

Bevor Sie auf die Messberichte in Collaboration zugreifen können, müssen Sie:

* [Verbinden](/help/guide/connect/establishing-connections.md) mit einem Mitarbeiter mit aktiviertem **Measurement**-Anwendungsfall
* Zusammenarbeit an mindestens einem Projekt mit dem Mitarbeiter. Erfahren Sie, wie [&#x200B; ein Projekt erstellen &#x200B;](/help/guide/collaborate/manage-projects.md#create-project).
* Führen Sie Ihre Kampagne aus und stellen Sie sicher[&#x200B; dass eine (Kampagnen-ID) für die Kampagne angegeben &#x200B;](../collaborate/manage-projects.md#manage-campaign-id):
   * Wenn Sie ein Publisher sind, geben Sie die Kampagnen-ID ein, die mit der Kampagne Ihres Advertisers verknüpft ist.
   * Wenn Sie ein Advertiser sind, bitten Sie Ihren Partner (Publisher), die Kampagnen-ID anzugeben. Dies ist erforderlich, um [Berichte im Messarbeitsbereich zu erstellen](#create-measurement-report).
* [Laden Sie &#x200B;](/help/guide/setup/onboard-measurement-data.md) in Collaboration hoch, wenn Sie [Attributionsberichte erstellen](#create-attribution-report).

## Anzeigen von Berichten {#view-reports}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_create_report_campaignID"
>title="Kampagnen-IDs"
>abstract="Platzhalter, um in der Benutzeroberfläche relevante Informationen über die Kampagnen-IDs hinzuzufügen."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_create_report"
>title="Kampagnen-IDs"
>abstract="Platzhalter, um in der Benutzeroberfläche relevante Informationen über die Kampagnen-IDs hinzuzufügen."

So zeigen Sie die auf der Registerkarte „Kennzahlen“ verfügbaren Berichte an:

1. Navigieren Sie zu **[!UICONTROL Zusammenarbeiten]** > **[!UICONTROL Meine Projekte]**.
2. Wählen Sie für Ihr gewünschtes Projekt &quot;**[!UICONTROL &quot;]**.
3. Wählen Sie im Projekt die Registerkarte **[!UICONTROL Kennzahlen]** aus.

Wählen Sie **[!UICONTROL Vollständigen Bericht anzeigen]**, um auf die verschiedenen verfügbaren Berichte zuzugreifen, die weiter unten beschrieben sind.

![So gelangen Sie zur Registerkarte „Messung“ in einem Projekt.](/help/assets/collaborate/measure/measurement.gif)

### Zusammenfassungsansicht

Die Seitenansicht oben auf der Registerkarte „Messung“ zeigt eine Kampagnenübersicht mit einigen allgemeinen Zahlen, auf die Sie verweisen können:

**[!UICONTROL Impressions]**: Die Gesamtzahl der Fälle, in denen das Kreative angezeigt wurde.
**[!UICONTROL Eindeutige Reichweite]**: Die Anzahl der individuellen Identitäten, die die kreative Seite gesehen haben.
**[!UICONTROL Durchschnittliche Gesamtfrequenz]**: Die Anzahl der Impressionen dividiert durch die erreichten eindeutigen Identitäten. Diese Zahl gibt an, wie oft jede Identität dem Kreativen angezeigt wurde.

![Ansicht der Kampagnenübersicht](/help/assets/collaborate/measure/campaign-summary.png)

### Metriken im Zeitverlauf {#metrics-over-time}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measure_metricsovertime"
>title="Metriken im Zeitverlauf"
>abstract="Verwenden Sie die Ansicht der Metriken im Zeitverlauf, um Informationen zur Gesamtanzahl der Impressionen zu erhalten, die während des Kampagnenzeitraums für Ihre Kreativen angezeigt wurden. Sie können maximal zwei Dimensionen auswählen, die im Bericht angezeigt werden sollen."

Verwenden Sie die Ansicht der Metriken im Zeitverlauf, um Informationen zur Gesamtanzahl der Impressionen zu erhalten, die während des Kampagnenzeitraums für Ihre Kreativen angezeigt wurden. Beachten Sie, dass Sie maximal zwei Metriken auswählen können, die im Bericht angezeigt und analysiert werden sollen.

![Ansicht der Metriken im Zeitverlauf.](/help/assets/collaborate/measure/metrics-over-time.png)

### Häufigkeitsverteilung {#frequency-distribution}

Verwenden Sie die Ansicht „Häufigkeitsverteilung“, um die Aufschlüsselung der Anzahl der Impressionen zu verstehen, die den einzelnen Benutzenden angezeigt wurden. Diese Ansicht kann Ihnen bei zukünftigen Kampagnen helfen, zu entscheiden, ab welchem Punkt Sie mit der Unterdrückung von Zielgruppen beginnen möchten. Beispielsweise können Sie Profile unterdrücken, die bereits dreimal einen Kreativen gesehen haben.

![Ansicht der Häufigkeitsverteilung.](/help/assets/collaborate/measure/frequency-distribution.gif)

### Metrik nach Dimension {#metric-by-dimension}

Analysieren Sie verschiedene Metriken wie Impressions, sichtbare Impressions, eindeutige Reichweite, Kosten und mehr im Kontext des Platzierungsmediums. Analysieren Sie, welches Medium (z. B. mobiles Streaming, CTV programmgesteuert oder andere) die besten Ergebnisse für Ihre Kampagnen erzielt.

![Metrik nach Dimension.](/help/assets/collaborate/measure/metric-by-dimension.png)

### Kurve der kumulativen Reichweiten {#cumulative-reach-curve}

Im Verlauf der Kampagne und der steigenden Anzahl von Impressionen wissen Sie, ob die Anzahl der Benutzenden, die Sie erreichen konnten, ebenfalls gestiegen ist. Ein gängiges Muster in Kampagnen besteht darin, dass nach einem bestimmten Punkt ein Plateau erreicht wird, in dem das Kreative denselben Personen immer wieder angezeigt wird. Diese Ansicht kann Ihnen dabei helfen, die Länge zukünftiger Kampagnen anzupassen, je nachdem, wann neue Personen nicht mehr erreicht werden.

![Kumulative Reichweitenkurve.](/help/assets/collaborate/measure/cumulative-reach-curve.png)

### Impressions nach Platzierung {#impressions-by-placement}

Erfahren Sie, welches Medium Eindrücke für Ihre Kreativen hervorruft. Dies kann Ihnen bei der Entscheidung helfen, wo Sie Ihre Werbeausgaben in zukünftige Kampagnen investieren sollten.

![Impressions nach Platzierung.](/help/assets/collaborate/measure/impressions-by-placement.png)

### Kumulative Konversionen {#cumulative-conversions}

Diese Ansicht bietet eine detaillierte Aufschlüsselung der Konversionsereignisse, die Sie messen möchten, im Tabellenformat. Die Tabelle enthält:

* **Konversionsereignis**: Name jedes Konversionsereignisses, das verfolgt wird.
* **Konversionsanzahl**: Gesamtanzahl der Konversionen, die für jedes Ereignis aufgetreten sind.
* **Geschätzter Umsatz**: Geschätzter Wert, der jedem Konversionsereignis zugeordnet wird.

Überprüfen Sie diese Tabelle, um die Effektivität Ihrer Kampagne bei der Unterstützung der gewünschten Aktionen zu bewerten.

![Kumulative Konversionen.](/help/assets/collaborate/measure/cumulative-conversions.png)

### Konversionen nach Tag {#conversions-by-day}

Dieses Diagramm enthält eine tägliche Aufschlüsselung der Konversionen für jedes Ereignis, das beim Erstellen eines Attributionsberichts eingerichtet wird. In dieser Ansicht können Sie tägliche Muster erkennen, Zeiten mit hoher oder geringer Konversionsaktivität identifizieren und die Leistung verschiedener Konversionsereignisse in Ihrer Kampagnenzeitleiste vergleichen.

![Konversionen nach Tag.](/help/assets/collaborate/measure/conversions-by-day.gif)

## Messbericht erstellen {#create-measurement-report}

In Collaboration können Sie zwei Haupttypen von Messberichten erstellen:

* **Kampagnenzusammenfassung** Bietet allgemeine Metriken wie Reichweite, Impressionen, durchschnittliche Häufigkeit und Versand nach Kanal, die einen schnellen Überblick über die allgemeine Kampagnenleistung geben.
* **Attribution**: Misst, wie Kampagnenbelichtungen nachgelagerte Aktionen wie Konversionen oder Käufe fördern, damit Sie die Effektivität von Kampagnen besser verstehen können.

Der Bericht „Kampagnenzusammenfassung“ kann eigenständig ausgeführt werden, während der Bericht „Attribution“ erfordert, dass beide Berichtstypen gemeinsam ausgewählt werden.

### Erstellen eines Zusammenfassungsberichts für eine Kampagne {#create-campaign-summary-report}

Sowohl Publisher als auch Advertiser können Berichte **Kampagnenübersicht)**, um die Kampagnenleistung zu bewerten. Verwenden Sie diese Berichte, um Einblicke in Schlüsselmetriken wie [Reichweite](#cumulative-reach-curve), [Häufigkeit](#frequency-distribution) und [Impressionen](#impressions-by-placement) zu erhalten und zu verstehen, wie Ihre Kampagne bereitgestellt wurde und wie sie sich insgesamt auswirkt.

Um einen Bericht **Kampagnenzusammenfassung** zu erstellen, navigieren Sie vom Arbeitsbereich **[!UICONTROL Mitarbeiter]** zum Projektarbeitsbereich. Wählen Sie auf der **[!UICONTROL Kennzahl]** das Symbol zum Hinzufügen aus (![Symbol hinzufügen.](/help/assets/icons/plus.png)) und wählen Sie dann **[!UICONTROL Messen]** aus.

Wenn dies Ihr erster Bericht ist, können Sie auch die Option **[!UICONTROL Bericht ausführen]** auswählen.

![Die Registerkarte „Kennzahlen“ mit hervorgehobenen Optionen „Bericht ausführen“ und „Kennzahlen“.](/help/assets/collaborate/measure/run-measure-report.png)

Der Bildschirm **[!UICONTROL Messbericht erstellen]** wird mit Informationen und Eingabefeldern angezeigt, die unter den Abschnitten **[!UICONTROL Abrechnungsdetails]**, **[!UICONTROL Kampagnendetails]** und **[!UICONTROL Berichtsdetails]** gruppiert sind.

#### Rechnungsdetails {#billing-details}

In diesem Abschnitt wird erläutert, wie Gutschriften bei der Erstellung von Messberichten verwendet werden. Die Zuständigkeit für das Guthaben wird während der [Verbindungseinrichtung](../connect/establishing-connections.md#credit-split) festgelegt. Bevor Sie Berichte ausführen, sollten Sie die Einstellungen für die Kreditaufteilung und die Berichterstellungsrollen mit Ihrem Mitarbeiter überprüfen und bestätigen.

#### Kampagnendetails {#campaign-details}

Wählen Sie im **[!UICONTROL Kampagnendetails]** die entsprechende (Advertiser **ID) aus** die mit Ihrem Bericht verknüpft werden soll. Diese Advertiser-Namen oder IDs wurden während der [Verbindungseinrichtung“ &#x200B;](../connect/establishing-connections.md#advertiser-names). Wenn nur ein Name konfiguriert wurde, wird er standardmäßig angezeigt. Wenn kein Name eingerichtet wurde, wird das Feld **[!UICONTROL Advertiser-ID (Name)]** deaktiviert und mit dem Advertiser-Kontonamen vorausgefüllt.

![Der Bildschirm „Messbericht erstellen“ mit deaktivierter Option „Advertiser-ID (Name)“.](/help/assets/collaborate/measure/advertiser-id.png)

Wählen Sie dann die gewünschte Kampagne aus dem Dropdown-Menü **[!UICONTROL Kampagnen-ID]** aus. In diesem Menü werden alle Kampagnen-IDs aufgelistet, die vom Publisher für Ihr Projekt eingegeben wurden. Wenn die benötigte Kampagne nicht verfügbar ist, [&#x200B; Sie sie in der Benutzeroberfläche &#x200B;](./manage-projects.md#manage-campaign-id), bevor Sie den Bericht erstellen.

![Der Bildschirm Messbericht erstellen , der das Dropdown-Menü Kampagnen-ID enthält, wird erweitert.](/help/assets/collaborate/measure/campaign-id.png)

Geben Sie als Nächstes den Zeitraum an, den der Bericht abdecken soll. Wählen Sie **[!UICONTROL Datumsbereich des Berichts]** und wählen Sie dann im Kalender das Start- und Enddatum aus.

![Der Bildschirm Messbericht erstellen zeigt den Datumsbereichskalender des Berichts.](/help/assets/collaborate/measure/report-date-range.png)

#### Berichtsdetails {#report-details}

**Ausführungsdatum des Berichts**

Wählen **[!UICONTROL Abschnitt „Berichtsdetails]** das Datum aus, an dem der Bericht ausgeführt werden soll. Wählen Sie **[!UICONTROL Ausführungsdatum des Berichts]** und wählen Sie Ihr bevorzugtes Datum aus dem Kalender aus.

* Wenn Sie das heutige Datum oder ein Datum in der Vergangenheit auswählen, wird der **Kampagnenübersicht** sofort ausgeführt.
* Wenn Sie ein Datum in der Zukunft auswählen **wird der Bericht** Kampagnenzusammenfassung) an diesem Tag ausgeführt.

![Der Bildschirm Messbericht erstellen zeigt den Kalender des Ausführungsdatums des Berichts.](/help/assets/collaborate/measure/report-run-date.png)

**Berichtstyp**

* Als Advertiser können Sie den Berichtstyp **[!UICONTROL Kampagnenübersicht]** aus den verfügbaren Optionen auswählen. Nur Werbetreibende können Attributionsberichte generieren.
* Wenn Sie Herausgeber sind, ist der Berichtstyp **[!UICONTROL Kampagnenübersicht]** vorausgewählt und kann nicht geändert werden. Zurzeit können Publisher keine Attributionsberichte ausführen.

![Der Bildschirm Messbericht erstellen zeigt die Option Kampagnenübersicht als vorausgewählten und unveränderlichen Berichtstyp an.](/help/assets/collaborate/measure/cs-report-type.png)

Überprüfen Sie abschließend Ihre Einstellungen und wählen Sie **[!UICONTROL Erstellen]** aus. Der Kampagnenübersichtsbericht wird sofort generiert, wenn das Ausführungsdatum heute oder früher oder am gewählten Datum in der Zukunft liegt. Sie können den terminierten Bericht vor dem Ausführungsdatum bearbeiten. Eine schrittweise Anleitung hierzu finden Sie im Abschnitt [Messbericht bearbeiten].

Sobald verfügbar, können Sie Ihren Bericht jederzeit auf der Registerkarte **[!UICONTROL Kennzahlen]** in Ihrem Projektarbeitsbereich anzeigen.

![Der Bildschirm „Messbericht erstellen“ mit hervorgehobenen Informationen und der hervorgehobenen Option „Erstellen“.](/help/assets/collaborate/measure/cs-review.png)

### Attributionsbericht erstellen {#create-attribution-report}

Als Advertiser können Sie **Attribution“-Berichte erstellen** um zu bewerten, wie Ihre Kampagnenrisiken zu wichtigen Ergebnissen wie Anmeldungen oder Käufen beitragen. Verwenden Sie diese Berichte, um Benutzerinteraktionen mit Ihrer Kampagne zu verstehen, zu ermitteln, welche Touchpoints die größte Wirkung erzielen, und um zu effektiveren Marketing-Strategien zu gelangen.

>[!IMPORTANT]
>
> Sie müssen [Ihre Messdaten in Collaboration &#x200B;](../setup/onboard-measurement-data.md#add-measurement-data), bevor Sie Attributionsberichte erstellen können.
>![Die Registerkarte Kennzahl mit den Anforderungen für Messdaten und der deaktivierten Option Kennzahl &#x200B;](/help/assets/collaborate/measure/require-measurement-data.png)

Um einen **Attributionsbericht** zu generieren, navigieren Sie vom Arbeitsbereich **[!UICONTROL Mitarbeiter]** zum Projektarbeitsbereich. Wählen Sie auf der **[!UICONTROL Kennzahl]** das Symbol zum Hinzufügen aus (![Symbol hinzufügen.](/help/assets/icons/plus.png)) und wählen Sie dann **[!UICONTROL Messen]** aus.

Wenn dies Ihr erster Bericht ist, können Sie auch die Option **[!UICONTROL Bericht ausführen]** auswählen.

![Die Registerkarte „Kennzahlen“ mit hervorgehobenen Optionen „Bericht ausführen“ und „Kennzahlen“.](/help/assets/collaborate/measure/run-measure-report-attribution.png)

Der Bildschirm **[!UICONTROL Messbericht erstellen]** wird mit Informationen und Eingabefeldern angezeigt, die unter den Abschnitten **[!UICONTROL Abrechnungsdetails]**, **[!UICONTROL Kampagnendetails]** und **[!UICONTROL Berichtsdetails]** gruppiert sind.

Lesen und befolgen Sie die Schritte im [Erstellen eines Kampagnenübersichtsberichts](#create-campaign-summary-report), um die folgenden Einstellungen zu konfigurieren:

* [Rechnungsdetails](#billing-details)
* [Kampagnendetails](#campaign-details)

#### Berichtsdetails für Attributionsberichte {#report-details-attribution}

**Ausführungsdatum des Berichts**

>[!IMPORTANT]
>
> Bei Attributionsberichten muss das Berichtslaufdatum ein künftiges Datum sein und mindestens einen Tag nach dem Enddatum Ihres Berichtsdatumsbereichs plus der vollständigen Dauer des definierten Lookback-Fensters liegen.
> **Ausführungsdatum ≥ Berichtsenddatum + Lookback-Fenster + 1**
> 
> Wenn Ihr Berichtsdatumsbereich beispielsweise am 15. Juni endet und das Lookback-Fenster 14 Tage beträgt, ist das Ausführungsdatum des Berichts der 30. Juni oder höher.

Wählen **[!UICONTROL Abschnitt „Berichtsdetails]** das Datum aus, an dem der Bericht ausgeführt werden soll. Wählen Sie **[!UICONTROL Ausführungsdatum des Berichts]** und wählen Sie Ihr bevorzugtes Datum aus dem Kalender aus.

**Berichtstyp**

Als Advertiser können Sie **[!UICONTROL Attribution]** als Berichtstyp zusätzlich zur **[!UICONTROL Kampagnenübersicht]** auswählen. Wenn Sie den Attributionsbericht auswählen, enthalten Ihre Ergebnisse sowohl standardmäßige Kampagnenübersichtsmetriken als auch eine detaillierte Attributionsanalyse, die eine umfassende Ansicht der Kampagnenleistung bietet.

![Der Bildschirm Messbericht erstellen mit den ausgewählten Berichtstypen für Kampagnenübersicht und Attribution.](/help/assets/collaborate/measure/attribution-report-type.png)

Wenn Sie **[!UICONTROL Attribution]** als Berichtstyp auswählen, wird ein Konfigurationsabschnitt **[!UICONTROL Attribution]** mit zusätzlichen erforderlichen Einstellungen angezeigt:

* **Lookback-Fenster in Tagen**: Legt fest, wie weit der Bericht vor jeder Konversion Kampagnen-Impressions berücksichtigt. Nur Impressionen innerhalb dieses Zeitraums sind für eine Attributions-Gutschrift geeignet.
* **Konversionsereignisse**: Gibt an, welche Konversionsaktionen Sie messen möchten, z. B. Käufe oder Anmeldungen. Diese Ereignisse müssen im Voraus eingerichtet werden, wenn Sie [Ihre Messdaten &#x200B;](../setup/onboard-measurement-data.md#add-conversion-event) Collaboration beziehen.

Geben Sie zunächst einen Wert für das Feld **[!UICONTROL Lookback-Fenster in Tagen]** ein oder passen Sie ihn mit den Optionen zum Erhöhen/Verringern an.

![Der Bildschirm „Messbericht erstellen“ mit Hervorhebung des Werts für das Lookback-Fenster in Tagen.](/help/assets/collaborate/measure/lookback-window-in-days.png)

Wählen Sie als Nächstes bis zu **3** Konversionsereignisse aus der verfügbaren Liste aus. Um weitere Informationen zu einem bestimmten Ereignis zu erhalten, klicken Sie auf das **[!UICONTROL i]**-Symbol, um dessen Details anzuzeigen.

![Der Bildschirm Messbericht erstellen mit den ausgewählten Konversionsereignissen und den Informationen zum Kaufereignis.](/help/assets/collaborate/measure/attribution-conversion-events.png)

Überprüfen Sie abschließend Ihre Einstellungen und wählen Sie **[!UICONTROL Erstellen]** aus, um den Bericht zu planen. Ihr Attributionsbericht wird am angegebenen Ausführungsdatum generiert. Sie können den terminierten Bericht vor dem Ausführungsdatum bearbeiten. Eine schrittweise Anleitung hierzu finden Sie im Abschnitt [Messbericht bearbeiten].

Sobald verfügbar, können Sie Ihren Bericht jederzeit auf der Registerkarte **[!UICONTROL Kennzahlen]** in Ihrem Projektarbeitsbereich anzeigen.

![Der Bildschirm „Messbericht erstellen“ mit hervorgehobenen Informationen und der hervorgehobenen Option „Erstellen“.](/help/assets/collaborate/measure/attribution-review.png)
