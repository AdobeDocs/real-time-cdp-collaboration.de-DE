---
title: Verfolgen der Kreditverbrauchsaktivität
description: Erfahren Sie, wie Sie die Kreditkonsumaktivität Ihres Unternehmens in Real-Time CDP Collaboration verfolgen.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
source-git-commit: b52fd181d80d5a70331571f7a4cbe3e5a7ec1d7c
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 1%

---

# Verfolgen der Kreditverbrauchsaktivität

{{limited-availability-release-note}}

>[!BEGINSHADEBOX]

**90-tägiger No-Overage-Zeitraum**: Kunden in förderfähigen Regionen profitieren von einem 90-tägigen No-Overage-Zeitraum ab dem Datum der Verfügbarkeit in ihrer Region. Während dieser Zeit fallen für die Überschreitung der Kreditberechtigung keine zusätzlichen Gebühren an.

>[!ENDSHADEBOX]

>[!IMPORTANT]
>
>Die Tabelle des Kreditverbrauchs wird zur Überwachung nach Tagen aufgerundet und aggregiert. Die Zahlen im Dashboard **[!UICONTROL Meine Aktivität]** stellen einen *geschätzten* Kreditverbrauch dar. Der *tatsächliche* Kreditverbrauch für die Abrechnung wird in internen Systemen verfolgt und steht Ihnen auf Anfrage zur Verfügung. Wenden Sie sich an den Adobe-Support, um diese Informationen zu erhalten.

Um auf die Aktivität Geschätzte Kreditnutzung zuzugreifen, gehen Sie im Hauptnavigationsmenü zu **[!UICONTROL Setup]** und wählen Sie dann die Registerkarte **[!UICONTROL Meine Aktivität]** aus.

![Mein Aktivitäts-Dashboard mit Details zum Kreditverbrauch](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>Die **[!UICONTROL Meine Aktivität]** enthält keine Informationen zu Benutzeraktionen in verschiedenen Bereichen der Benutzeroberfläche von Real-Time Collaboration CDP. Verwenden Sie die [Auditprotokolle](/help/guide/setup/audit-logs.md), um diese Informationen abzurufen.

## Grundlegendes zum Aktivitäts-Dashboard {#understand-dashboard}

Das Aktivitäts-Dashboard zeigt eine umfassende Liste aller kreditverbrauchenden Vorgänge in Ihrem Unternehmen an. Jede Zeile stellt eine eigene Aktivität dar und enthält wichtige Informationen zur Kreditverwendung:

>[!NOTE]
>
>**[!UICONTROL Zielgruppen-Management]**-Aktivitäten sind keinem anderen Mitarbeiter zugeordnet. Daher geben die Spalten **[!UICONTROL Verbindungs-ID]** und **[!UICONTROL Verbindungsname]** für diese Aktivitätstypen einen **[!UICONTROL K/A]**-Wert an.

| Spalte | Beschreibung |
|------------|--------------|
| **[!UICONTROL Datum]** | Das Datum, an dem die Aktivität stattfand, angezeigt im Format MM/TT/JJJJ. |
| **[!UICONTROL Verbindungs-ID]** | Eine eindeutige Kennung für jede Verbindung, die mit einer kreditverbrauchenden Aktivität verbunden ist, dargestellt als alphanumerische Zeichenfolge. |
| **[!UICONTROL Verbindungsname]** | Der Name des Mitarbeiters, der mit der Verbindung und der kreditverbrauchenden Aktivität verknüpft ist. |
| **[!UICONTROL Aktivität]** | Der Typ der durchgeführten Aktivität, z. B **„Aktivierung - Abgleich**, **Aktivierung -**&quot; oder **Zielgruppenverwaltung**. |
| **[!UICONTROL Eingaben verarbeitet]** | Die Gesamtzahl der für die Aktivität verarbeiteten Eingaben (z. B. IDs oder Zeilen). |
| **[!UICONTROL Insgesamt verwendete Guthaben]** | Die Gesamtzahl der von der Aktivität verwendeten Credits. |
| **[!UICONTROL Meine Kreditaktie]** | Der Anteil Ihres Unternehmens an den für die Aktivität verwendeten Guthaben. |

{style="table-layout:auto"}

## Aktivitätstypen {#types-of-activities}

Die Spalte **[!UICONTROL Aktivität]** zeigt verschiedene Arten von kreditverbrauchenden Vorgängen.

* **[!UICONTROL Zielgruppen-Management]**: Guthaben werden genutzt, wenn Zielgruppen in Real-Time CDP Collaboration bezogen werden. Die Credits werden als Funktion der Anzahl der in Real-Time CDP Collaboration über alle Zielgruppen hinweg indizierten IDs (in Millionen) und der Häufigkeit dieser Indizierung (täglich, alle drei Tage oder wöchentlich) genutzt. Weitere Informationen finden Sie im Handbuch [Importieren und Verwalten ](/help/guide/setup/onboard-audiences.md) Zielgruppen“.
* **[!UICONTROL Aktivierung - Abgleich]** - Gutschriften werden in Abhängigkeit von der Anzahl der übereinstimmenden und für die Aktivierung vorbereiteten IDs genutzt. Weitere Informationen finden Sie im Handbuch [Aktivieren von Zielgruppen](/help/guide/collaborate/activate.md).
* **[!UICONTROL Aktivierung - Ausgang]** - Guthaben wird in Abhängigkeit von der Anzahl der IDs genutzt, die an ein Ziel gesendet werden. Dies wird immer dem Mitarbeiter berechnet, der die Zielgruppe erhält. Weitere Informationen finden Sie im Handbuch [Aktivieren von Zielgruppen](/help/guide/collaborate/activate.md).
* **[!UICONTROL Messung]** - Führen Sie Aktivitäten in Real-Time CDP Collaboration aus, um Leistungsberichte und Einblicke für Kampagnen zu generieren. Die Credits werden basierend auf der Anzahl der Zeilen in Kampagnenberichten über alle Kampagnen hinweg und der Häufigkeit der Berichterstellung (täglich, alle drei Tage oder wöchentlich) genutzt.

## Kreditnutzung verwalten {#manage-credit-consumption}

So verwalten Sie Ihren Kreditverbrauch effektiv:

1. **Verstehen** Der mit jeder Aktivität verknüpfte Kreditverbrauch. In der [Real-Time CDP Collaboration-Produktbeschreibung](https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank} finden Sie eine Tabelle mit den für die Zusammenarbeit verwendeten Credits pro Aktivität.
2. **Regelmäßig überwachen**: Überprüfen Sie Ihr Aktivitäts-Dashboard häufig, um Nutzungsmuster zu verstehen.
3. **Nach Verbindung verfolgen**: Verwenden Sie den Verbindungsnamen, um zu ermitteln, welche Partnerschaften die meisten Credits verbrauchen.

<!--

## Pagination and navigation

The activity list is paginated to improve performance and readability. Use the navigation controls at the bottom of the table to move between pages and adjust how many records you can view at once.

-->
