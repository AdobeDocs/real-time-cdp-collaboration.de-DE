---
title: Leistung messen
description: Messen Sie die Leistung Ihrer Kampagnen über verschiedene Kanäle hinweg. Erfahren Sie, wie Sie verschiedene Berichte verwenden und interpretieren.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
source-git-commit: b52fd181d80d5a70331571f7a4cbe3e5a7ec1d7c
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 18%

---

# Leistung messen

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>Der **[!UICONTROL Measure]**-Arbeitsbereich ist nur verfügbar, wenn der **Measurement**-Anwendungsfall [während des Verbindungsprozesses) ](../connect/establishing-connections.md#connection-settings) wurde. Weitere Informationen zu Anwendungsfällen finden Sie im Handbuch [Verwalten von ](./manage-projects.md#project-use-cases)&quot;.

Erfahren Sie mehr über die verfügbaren Berichte in Real-Time CDP Collaboration und lernen Sie, wie Sie die Leistung Ihrer Marketing-Kampagnen kanalübergreifend messen und analysieren können.

## Voraussetzungen

Bevor Sie auf die Messberichte in Real-Time CDP Collaboration zugreifen können, haben Sie bereits Folgendes getan:

* [Verbunden](/help/guide/connect/establishing-connections.md) mit einem gewünschten Advertiser oder Publisher, für den der **Measurement**-Anwendungsfall aktiviert ist und der mit der Zusammenarbeit an [Projekten](/help/guide/collaborate/manage-projects.md)
* Führen Sie eine Kampagne aus und [hochgeladene Messdaten](/help/guide/setup/onboard-measurement-data.md) in Real-Time CDP Collaboration.

<!--

## Create a report {#create-report}

Hidden until functionality is live. At that point, move the contextualhelp from below into this section. 

The syntax rtcdp_collaboration_measurement_create_report is currently implemented in the UI. However, a preference would be to imlement the other contextualhelp ID from below instead, since that explicitly includes campaignID in the syntax. Need to sync up with UI team. More details in CORE-116991.

-->

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

### Impressionen nach Platzierung {#impressions-by-placement}

Erfahren Sie, welches Medium Eindrücke für Ihre Kreativen hervorruft. Dies kann Ihnen bei der Entscheidung helfen, wo Sie Ihre Werbeausgaben in zukünftige Kampagnen investieren sollten.

![Impressions nach Platzierung.](/help/assets/collaborate/measure/impressions-by-placement.png)

## Nächste Schritte

![Entdecken, aktivieren, messen für Werbetreibende.](/help/assets/end-to-end-workflow/discover-activate-measure.png)

Nutzen Sie im Sinne der oben gezeigten Zyklizität bei der Planung Ihrer nächsten Kampagne die Einblicke, die Sie durch die Anzeige der Berichte erhalten haben. Wenn Sie als Werbetreibender erforderlich sind, gehen Sie zurück, um verschiedene Herausgeber zu entdecken, und führen Sie Überschneidungen aus, um verschiedene Zielgruppen für Ihre nächsten Kampagnen zu entdecken.
