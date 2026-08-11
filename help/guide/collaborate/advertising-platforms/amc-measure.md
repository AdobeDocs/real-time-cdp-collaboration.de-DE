---
title: Erstellen von Amazon Marketing Cloud-Messberichten
description: Erfahren Sie, wie Sie Messberichte für Amazon Marketing Cloud-Kampagnen in Real-Time CDP Collaboration erstellen und interpretieren.
audience: advertiser
keywords: AMC, Amazon Marketing Cloud, Messberichte, Kampagnenübersicht, Attribution, Real-Time CDP Collaboration
solution: Real-Time Customer Data Platform Collaboration
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 944914557c10b43abbe4915e061c219aca9f783f
workflow-type: tm+mt
source-wordcount: '1574'
ht-degree: 5%

---


# Erstellen [!DNL Amazon Marketing Cloud] Messberichten {#amc-measurement-reports}

{{limited-availability-release-note}}

Verwenden Sie die **[!UICONTROL Kennzahlen]** in einem [!DNL Amazon Marketing Cloud] ([!DNL AMC])-Projekt, um die Reichweite, Häufigkeit und Konversionsergebnisse der Zielgruppe zu überprüfen. Nachdem Sie ein AMC-Projekt erstellt haben, erstellen Sie Messberichte für Kampagnen, die bereits ausgeführt wurden, und verwenden Sie dazu die in Ihrer [!DNL AMC]-Instanz verfügbaren Daten.

>[!IMPORTANT]
>
>Auf **[!UICONTROL Registerkarte]** Kennzahlen“ wird „Keine Messdaten verfügbar“ angezeigt, bis die Einrichtungsabfragen für die Hintergrunddaten abgeschlossen sind. Dieser Vorgang kann bis zu 24 Stunden dauern. Wenn die Meldung nach 24 Stunden weiterhin angezeigt wird, lesen Sie den Abschnitt [Fehlerbehebung](#troubleshooting).


## Erstellen eines Berichts {#create-report}

Gehen Sie wie folgt vor, um einen [!DNL AMC]-Messbericht [Erstellen eines Kampagnenübersichtsberichts](../measure.md#create-campaign-summary-report-create-campaign-summary-report) zu erstellen.

![Das Formular des Messberichts, das die Felder Advertiser-ID, Kampagnen-ID-Dropdown, Datumsbereich des Berichts, Ausführungsdatum des Berichts, Berichtsname und Berichtstyp enthält.](../../../assets/collaborate/advertising-platforms/create-measurement-report.png){zoomable="yes"}

### Kampagnendetails {#campaign}

Mit **[!UICONTROL Advertiser-ID]** wird das mit der [!DNL AMC]-Instanz verknüpfte [!DNL Amazon Advertising]-Konto identifiziert. [!DNL AMC] verwendet diesen Kontenkontext, um Kampagnen für die Messung abzurufen.

Die **[!UICONTROL Kampagnen-ID]**-Liste wird automatisch mit Kampagnen gefüllt, die in der verbundenen [!DNL AMC]-Instanz verfügbar sind. Eine Kampagne wird nur angezeigt, wenn sie in das standardmäßige Discovery-Lookback-Fenster fällt und über genügend eindeutige Benutzer verfügt, um den Mindestaggregationsschwellenwert von [!DNL AMC] zu erfüllen. Wählen Sie die Kampagne aus, deren [!DNL Amazon Ads] gemessen werden soll.

Wenn die benötigte Kampagne nicht aufgeführt ist, stellen Sie sicher, dass sie zum verbundenen [!DNL Amazon Ads]-Konto gehört, und überprüfen Sie [Fehlerbehebung](#troubleshooting). Weitere Informationen zu diesem Schwellenwert finden Sie in der Dokumentation [AMC-Aggregationsschwellenwert](https://advertising.amazon.com/API/docs/en-us/guides/amazon-marketing-cloud/aggregation-threshold).

#### Datumsbereich, Ausführungsdatum und Berichtsname {#dates}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_measure_report_date_range"
>title="Datumsbereich"
>abstract="Legen Sie das Start- und Enddatum für die Kampagnendaten fest, die in den Bericht aufgenommen werden sollen. Der Datumsbereich ist auf ein 365-tägiges Lookback-Fenster mit einer maximalen Spanne von 90 Tagen beschränkt. Sie können nur Berichte zu früheren Kampagnen erstellen."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_measure_report_run_date"
>title="Ausführungsdatum"
>abstract="Das Datum der Berichtsausführung. Muss mindestens einen Tag nach dem Enddatum des Berichts liegen und kann bis zu 46 Tage in der Zukunft liegen."

>[!NOTE]
>
>Sie können nur Berichte zu Kampagnen erstellen, die bereits ausgeführt wurden.

Legen Sie den **[!UICONTROL Datumsbereich des Berichts]** auf den Zeitraum fest, in dem die ausgewählte [!DNL AMC]-Kampagne ausgeführt wurde. [!DNL AMC] unterstützt ein 365-tägiges Lookback-Fenster mit einer maximalen Spanne von 90 Tagen.

Legen Sie das **[!UICONTROL Ausführungsdatum des Berichts]** fest. Dies ist das Datum der Berichtsausführung. Das Ausführungsdatum muss mindestens einen Tag nach dem Berichtsenddatum liegen und kann bis zu 46 Tage in der Zukunft liegen. Eine vollständige Liste der Datumsbeschränkungen finden Sie unter [AMC Constraints Reference](#constraints).

>[!TIP]
>
>Legen Sie für Attributionsberichte, bei denen der Datumsbereich innerhalb von 30 Tagen ab dem aktuellen Datum liegt, das Ausführungsdatum auf 30 Tage in der Zukunft fest, um sicherzustellen, dass alle Konversionen innerhalb des festen 30-tägigen Lookback-Fensters erfasst wurden, bevor der Bericht ausgeführt wird.

#### Berichtstyp {#report-type}

Alle [!DNL AMC] Berichte enthalten eine **[!UICONTROL Kampagnenübersicht]**. Optional können Sie Daten vom Typ **[!UICONTROL Attribution]** einbeziehen, um zu messen, ob Kampagnenimpressionen zu Kundenaktionen wie Käufen oder Anmeldungen innerhalb eines 30-Tage-Fensters nach der Offenlegung von Werbung geführt haben. Für die Attribution müssen die entsprechenden Konversionsereignisse in Ihrer [!DNL AMC]-Instanz verfügbar sein. Für Kampagnen, die sich auf Reichweite oder Bekanntheit **[!UICONTROL , enthält die]** Kampagnenübersicht“ die benötigten Versandmetriken.

| Berichtstyp | Beschreibung |
| --- | --- |
| **[!UICONTROL Kampagnenübersicht]** | Bietet Metriken zu Reichweite, Häufigkeit und Impression für die ausgewählte Kampagne. Immer eingeschlossen. |
| **[!UICONTROL Attribution]** | Fügt dem Bericht Konversionsdaten hinzu. Nur verfügbar, wenn Konversionsereignisse in Ihrer [!DNL AMC] vorhanden sind. Siehe [Konversionsereignisse](#conversion-events). |

#### Konversionsereignisse (nur Attribution) {#conversion-events}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_attribution_lookback_period"
>title="Lookback-Zeitraum für Attribution"
>abstract="AMC erzwingt ein festes Attributionsfenster von 30 Tagen: Konversionen, die bis zu 30 Tage nach der letzten Impression auftreten, können Impressions innerhalb des Datumsbereichs des Berichts zugewiesen werden. Dieser Wert kann nicht bearbeitet werden. Planen Sie das Ausführungsdatum des Berichts mindestens 30 Tage nach dem Ende des Zeitraums, um sicherzustellen, dass alle zulässigen Konversionen erfasst werden."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_measure_conversion_events"
>title="Konversionsereignisse"
>abstract="Wählen Sie bis zu drei Konversionsereignisse aus, die in den Attributionsbericht aufgenommen werden sollen. Verfügbare Ereignisse werden automatisch von Ihrer [!DNL AMC]-Instanz erkannt. Wenn keine Ereignisse angezeigt werden, sind in Ihrer [!DNL AMC]-Instanz möglicherweise keine Konversionsereignisse aufgezeichnet und die Attribution ist nicht verfügbar."

>[!NOTE]
>
>Attributionsdaten erfordern, dass Konversionsereignisse in Ihrer [!DNL AMC]-Instanz konfiguriert werden. Wenn [!UICONTROL Attribution] nicht verfügbar oder nicht ausgewählt war, überspringen Sie diesen Abschnitt und wählen Sie **[!UICONTROL Erstellen]** aus, um das Formular zu senden.

Für [!UICONTROL Attribution]-Berichte wendet [!DNL AMC] ein festes 30-tägiges Attribution-Lookback-Fenster an. Diese Einstellung kann nicht angepasst werden.

![Der Abschnitt Konversionsereignisse des Messberichts-Formulars in seinem aktiven Zustand, in dem das Feld „Lookback-Fenster“ auf 30 Tage eingestellt ist und die Mehrfachauswahlliste „Konversionsereignisse“ mit verfügbaren Ereignissen angezeigt wird.](../../../assets/collaborate/advertising-platforms/conversion-events-active.png){zoomable="yes"}

Konversionsereignisse stellen Kundenaktionen auf der Site dar, die von [!DNL Amazon Ads] verfolgt werden, z. B. einen Kauf, das Hinzufügen einer Wunschliste, eine Aktion zum Warenkorb oder eine Produktdetailansicht. Attributionsberichte unterstützen bis zu drei Ereignisse. Wählen Sie die Ereignisse aus, die den zu messenden Kampagnenergebnissen entsprechen. Wenn die Option [!UICONTROL Attribution] nicht verfügbar ist, finden Sie weitere Informationen unter [Fehlerbehebung](#troubleshooting).

Nachdem Sie den Bericht erstellt haben, wird er auf der Registerkarte **[!UICONTROL Kennzahlen]** mit dem Status Geplant oder Ausstehend angezeigt. Am konfigurierten Ausführungsdatum verarbeitet [!DNL AMC] die Berichtsabfrage und gibt die Ergebnisse innerhalb von 24 Stunden zurück.

![Die Registerkarte Kennzahlen zeigt eine neu erstellte Messberichtkarte mit der Statusanzeige Geplant , den Berichtsnamen, das Ausführungsdatum und den Berichtstyp sind sichtbar.](../../../assets/collaborate/advertising-platforms/measurement-report-pending.png){zoomable="yes"}


## Anzeigen eines Berichts {#view-report}

Sobald ein Bericht ausgeführt wurde, sind die Ergebnisse auf der Registerkarte **[!UICONTROL Kennzahlen]** des [!DNL AMC]-Projekts verfügbar. Suchen Sie Ihren Bericht und wählen Sie **[!UICONTROL Vollständigen Bericht anzeigen]**, um die Ergebnisse zu überprüfen.

![Die Registerkarte „Kennzahlen“ in einem [!DNL AMC]-Projekt zeigt eine abgeschlossene Berichtskarte mit dem Ausführungsdatum, dem Berichtstyp und der hervorgehobenen Schaltfläche „Vollständigen Bericht anzeigen“.](../../../assets/collaborate/advertising-platforms/view-full-report.png){zoomable="yes"}

Der Bericht zeigt die für den ausgewählten Berichtstyp verfügbaren Ergebnisse an. **[!UICONTROL Kampagnenzusammenfassung]** Berichte zeigen die Versandergebnisse für die ausgewählte Amazon-Kampagne an.

![Die Visualisierungen der Kampagnenübersicht, die Zusammenfassungssummen, die Impressions-Verteilung, die Häufigkeitsverteilung, die Reichweitenkurve und Impressions nach Platzierung anzeigen.](../../../assets/collaborate/advertising-platforms/campaign-summary-widgets.png){zoomable="yes"}

Berichte, die **[!UICONTROL Attribution]** enthalten, zeigen auch die Konversionsaktivität, die mit den ausgewählten Amazon Ads-Konversionsereignissen verknüpft ist.


![Die Attributionsvisualisierungen zeigen die Diagramme Kumulative Konversionen und Konversionen nach Tag.](../../../assets/collaborate/advertising-platforms/attribution-report-conversion-widgets.png){zoomable="yes"}

Weitere Informationen zur Interpretation der Berichtsergebnisse finden Sie unter [Leistung messen](../measure.md#view-reports-view-reports).

## [!DNL AMC] {#constraints}

Die folgenden Einschränkungen gelten für alle [!DNL AMC] Messberichte.

| Beschränkung | Wert |
| --- | --- |
| Frühester Beginn des Datumsbereichs des Berichts | 365 Tage vor dem aktuellen Datum |
| Ende des letzten Berichtsdatumsbereichs | 45 Tage nach dem aktuellen Datum. Damit können Sie einen Bericht für eine Kampagne vorkonfigurieren, die noch läuft und in den nächsten 45 Tagen abgeschlossen werden soll. Der Bericht wird automatisch am geplanten Ausführungsdatum nach dem Ende der Kampagne ausgeführt. |
| Maximaler Datumsbereich des Berichts | 90 Tage |
| Attributions-Lookback-Fenster | 30 Tage (für [!DNL AMC] festgelegt) |
| Mindestdatum der Ausführung | Mindestens 1 Tag nach dem Enddatum des Berichts |
| Maximales Ausführungsdatum | In 46 Tagen |
| Maximale Anzahl an Konversionsereignissen pro Bericht | 3 |
| Kampagnenauswahl | Einzelne Kampagne pro Bericht |
| Berichtbearbeitung | Nicht verfügbar. Der vorhandene Bericht wird beibehalten. [Neuen Bericht erstellen](#create-report) wenn Änderungen erforderlich sind |

## Fehlerbehebung {#troubleshooting}

**Keine Messdaten verfügbar**

Die **[!UICONTROL Kennzahl]** zeigt „Keine Messdaten verfügbar“ an, bis die bei der Projekterstellung ausgelösten Abfragen zur Einrichtung der Hintergrunddaten abgeschlossen sind. Dies kann bis zu 24 Stunden dauern. Wenn die Meldung „Keine Messdaten verfügbar“ nach 24 Stunden angezeigt wird, stellen Sie sicher, dass Ihre [!DNL AMC]-Instanz über Kampagnen verfügt, die innerhalb der letzten drei Monate ausgeführt wurden, da dies das Standard-Lookback-Fenster ist, das bei der Kampagnenerkennung verwendet wird. Wenn geeignete Kampagnen vorhanden sind und die Nachricht weiterhin besteht, überprüfen Sie Ihren Kampagnenstatus in Ihrem [Amazon Ads-Konto](https://advertising.amazon.com/sign-in){target="_blank"}.

**In der Dropdown-Liste [!UICONTROL Kampagnen-ID] werden keine Kampagnen angezeigt**

Kampagnen können auch dann fehlen, wenn die Registerkarte **[!UICONTROL Kennzahlen]** angezeigt wird. [!DNL AMC] wendet einen Mindestbenutzerschwellenwert auf Kampagnendaten an. Kampagnen, die den Mindestschwellenwert für eindeutige Benutzer nicht erreichen, werden ausgeschlossen und Berichtsabfragen geben keine Ergebnisse zurück. Stellen Sie sicher, dass die Kampagnen, über die Sie einen Bericht erstellen möchten, ausreichend Reichweite haben. Weitere Informationen zu den Aggregationsschwellenwerten von [!DNL AMC] finden Sie in der Dokumentation [AMC-Aggregationsschwellenwerte](https://advertising.amazon.com/API/docs/en-us/guides/amazon-marketing-cloud/aggregation-threshold){target="_blank"}.

**Ergebnisse sind nach dem Ausführungsdatum nicht mehr sichtbar**

Warten Sie bis zu 24 Stunden nach dem geplanten Ausführungsdatum, damit [!DNL AMC] die Berichtsabfragen verarbeiten und Ergebnisse zurückgeben kann. Wenn der Bericht nach diesem Zeitraum ausstehend bleibt, überprüfen Sie, ob das Ausführungsdatum abgelaufen ist und der Berichtsstatus nicht mehr als ausstehend angezeigt wird.

**Konversionsereignisse sind nicht verfügbar und [!UICONTROL Attribution] ist ausgegraut**

Dies kann aus drei Gründen auftreten:

1. **Konversionsverfolgung ist nicht aktiviert.** Für Ihr [!DNL AMC] Advertiser-Konto ist möglicherweise kein Konversions-Tracking konfiguriert. Navigieren Sie zu Ihrem [Amazon Ads](https://advertising.amazon.com/sign-in){target="_blank"}Konto und vergewissern Sie sich, dass Konversionsereignisse für die entsprechenden Kampagnen verfolgt werden.
2. **Keine aufgezeichneten Konversionsereignisse.** Selbst bei aktiviertem Tracking hat Ihre [!DNL AMC]-Instanz möglicherweise noch keine Konversionsereignisse aufgezeichnet.
3. **Aggregationsschwellenwert nicht erreicht.** [!DNL AMC] wendet einen Mindestschwellenwert auf Konversionsdaten an. Wenn ein Konversionsereignistyp nicht über eine ausreichende Anzahl von Vorkommen verfügt, wird er nicht zurückgegeben und nicht in der Liste angezeigt.

**Konversionen scheinen niedriger als erwartet**

Wenn das Ausführungsdatum des Berichts weniger als 30 Tage nach dem Ende des Datumsbereichs liegt, haben [!DNL AMC] möglicherweise nicht alle Konversionen innerhalb des Attributionsfensters erfasst. [Neuen Bericht erstellen](#create-report) mit einem Ausführungsdatum, das mindestens 30 Tage nach dem Ende des Datumsbereichs liegt.

## Nächste Schritte {#next-steps}

Verwenden Sie die Berichtsergebnisse, um die Leistung einer Kampagne zu bewerten und Informationen für die zukünftige Kampagnenplanung in [!DNL Amazon Advertising] zu erhalten. Sie können beispielsweise die Zielgruppenbestimmung anpassen, überbelichtete Zielgruppen, die in der Häufigkeitsverteilung identifiziert wurden, unterdrücken oder Ausgaben leistungsstarken Platzierungen zuweisen. Um eine andere Kampagne oder einen anderen Berichtszeitraum zu analysieren, erstellen Sie einen weiteren Messbericht mit den entsprechenden Einstellungen.

Einen Überblick über alle verfügbaren Funktionen zur [!DNL AMC]-Zusammenarbeit finden Sie unter [[!DNL Amazon Marketing Cloud]](./amc.md).
