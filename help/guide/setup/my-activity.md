---
title: Verfolgen Ihrer Kreditnutzungsaktivität
description: Erfahren Sie, wie Sie die Credit Wallet Ihres Unternehmens anzeigen und die Aktivität zur Kreditaufnahme in Real-Time CDP Collaboration verfolgen können.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
TQID: https://experienceleague.adobe.com/hDvkKFUCBYvsX8wntcYFrL6qZTxOo5CZOWAbxNwk7mw
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 681f4af47a58a2ce66b25b09d793d0b5b127df39
workflow-type: tm+mt
source-wordcount: 726
ht-degree: 2%

---

# Verfolgen Ihrer Kreditnutzungsaktivität {#track-credit-consumption-activity}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_my_activity"
>title="Mehr dazu"
>abstract=""

{{limited-availability-release-note}}

>[!BEGINSHADEBOX]

**90-tägiger No-Overage-Zeitraum**: Kunden in förderfähigen Regionen profitieren von einem 90-tägigen No-Overage-Zeitraum ab dem Datum der Verfügbarkeit in ihrer Region. Während dieser Zeit fallen für die Überschreitung der Kreditberechtigung keine zusätzlichen Gebühren an.

>[!ENDSHADEBOX]

Um auf Ihre Aktivität „Kreditbrieftasche“ und „Kreditverbrauch“ zuzugreifen, navigieren Sie **[!UICONTROL Hauptnavigation zu]** Setup“ und wählen Sie dann die Registerkarte **[!UICONTROL Meine Aktivität]** aus.

![Die Registerkarte „Meine Aktivität“ mit der Kreditbrieftasche mit bereitgestellten Guthaben, verbrauchten Guthaben, verfügbaren Guthaben und der Aktivitätstabelle für den Kreditverbrauch.](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>Die **[!UICONTROL Meine Aktivität]**-Ansicht enthält keine Benutzeraktionen aus anderen Bereichen der Real-Time CDP Collaboration-Benutzeroberfläche. Verwenden Sie die [Auditprotokolle](/help/guide/setup/audit-logs.md), um diese Informationen abzurufen.

## Die Ansicht „Meine Aktivität“ {#understand-dashboard}

Verwenden Sie die Ansicht **[!UICONTROL Meine Aktivität]**, um Ihre Kreditnutzung zu überwachen und die Aktivitäten zu überprüfen, die Kredite verbrauchen. Die Ansicht enthält die Credit Wallet und eine Aktivitätstabelle.

Die Credit Wallet zeigt Ihre bereitgestellten Guthaben, verbrauchten Guthaben und verfügbaren Guthaben an.

| Metrik | Beschreibung |
|---------|-------------|
| **[!UICONTROL Guthaben bereitgestellt]** | Die Anzahl der für Ihr Konto bereitgestellten Guthaben. |
| **[!UICONTROL Genutzte Guthaben]** | Die Anzahl der Guthaben, die von Ihrem Konto zum Zeitpunkt der letzten täglichen Aktualisierung verbraucht wurden. |
| **[!UICONTROL Verfügbare Guthaben]** | Die Anzahl der Ihrem Konto zur Verfügung stehenden Guthaben, berechnet aus bereitgestellten Guthaben minus verbrauchten Guthaben. |

{style="table-layout:auto"}

In der Tabelle Aktivität werden die täglichen Einträge zur Kreditaufnahme nach Datum, Aktivitätstyp, verarbeiteten Eingaben und verwendeten Gutschriften aufgelistet:

>[!NOTE]
>
>**[!UICONTROL Zielgruppen-Management]**-Aktivitäten sind keinem anderen Mitarbeiter zugeordnet, sodass die Spalten **[!UICONTROL Verbindungs-ID]** und **[!UICONTROL Verbindungsname]** für diese Aktivitätstypen einen **[!UICONTROL -]** Wert anzeigen.

| Spalte | Beschreibung |
|------------|--------------|
| **[!UICONTROL Datum]** | Das Datum, an dem die Aktivität stattfand, angezeigt im Format MM/TT/JJJJ. |
| **[!UICONTROL Verbindungs-ID]** | Eine eindeutige Kennung für jede Verbindung, die mit einer kreditverbrauchenden Aktivität verbunden ist, dargestellt als alphanumerische Zeichenfolge. |
| **[!UICONTROL Verbindungsname]** | Der Name des Mitarbeiters, der mit der Verbindung und der kreditverbrauchenden Aktivität verknüpft ist. |
| **[!UICONTROL Aktivität]** | Der Typ der durchgeführten Aktivität, z. B **[!UICONTROL „Aktivierung - Zielgruppenzugriff (einmal)]**, **[!UICONTROL Aktivierung - Zielgruppenzugriff (wiederkehrend)]**, **[!UICONTROL Aktivierung - Zielgruppenausgang (einmal)]**, **[!UICONTROL Aktivierung - Zielgruppenausgang (wiederkehrend)]** oder **[!UICONTROL Zielgruppenverwaltung]**. |
| **[!UICONTROL Eingaben verarbeitet]** | Die Gesamtzahl der für die Aktivität verarbeiteten Eingaben (z. B. IDs oder Zeilen). |
| **[!UICONTROL Insgesamt verwendete Guthaben]** | Die gesamten von der Aktivität verwendeten Guthaben. |
| **[!UICONTROL Meine Kreditaktie]** | Der Anteil Ihres Kontos an den für die Aktivität verwendeten Guthaben. |

{style="table-layout:auto"}

## Aktivitätstypen {#types-of-activities}

Die Spalte **[!UICONTROL Aktivität]** zeigt verschiedene Arten von kreditverbrauchenden Vorgängen.

* **[!UICONTROL Zielgruppen-Management]**: Guthaben werden genutzt, wenn Zielgruppen in Collaboration bezogen werden. Die Guthaben werden als Funktion der Anzahl der in Collaboration indizierten IDs für alle Zielgruppen und der Häufigkeit dieser Indizierung genutzt, z. B. täglich, alle drei Tage oder wöchentlich. Weitere Informationen finden Sie im Handbuch [Beschaffung und Verwaltung &#x200B;](/help/guide/setup/onboard-audiences.md) Zielgruppen“.
* **[!UICONTROL Aktivierung - Zielgruppenzugriff (einmal)]**: Guthaben werden verbraucht, wenn der Zielgruppenzugriff einmal über den Aktivierungs-Workflow verarbeitet wird. Weitere Informationen finden Sie im Handbuch [Aktivieren von Zielgruppen](/help/guide/collaborate/activate.md).
* **[!UICONTROL Aktivierung - Zielgruppenzugriff (wiederkehrend)]**: Credits werden verwendet, wenn der Zielgruppenzugriff über den Aktivierungs-Workflow nach einem wiederkehrenden Zeitplan verarbeitet wird. Weitere Informationen finden Sie im Handbuch [Aktivieren von Zielgruppen](/help/guide/collaborate/activate.md).
* **[!UICONTROL Aktivierung - Zielgruppenausgang (einmal)]**: Guthaben werden verbraucht, wenn der Zielgruppenausgang an ein Ziel einmal durch den Aktivierungs-Workflow verarbeitet wird. Diese Aktivität wird dem Mitarbeiter berechnet, der die Zielgruppe erhält. Weitere Informationen finden Sie im Handbuch [Aktivieren von Zielgruppen](/help/guide/collaborate/activate.md).
* **[!UICONTROL Aktivierung - Zielgruppenausgang (wiederkehrend)]**: Credits werden verwendet, wenn Zielgruppenausgang an ein Ziel über den Aktivierungs-Workflow in einem wiederkehrenden Zeitplan verarbeitet wird. Diese Aktivität wird dem Mitarbeiter berechnet, der die Zielgruppe erhält. Weitere Informationen finden Sie im Handbuch [Aktivieren von Zielgruppen](/help/guide/collaborate/activate.md).
* **[!UICONTROL Messung]**: Guthaben wird verbraucht, wenn Sie in Collaboration Leistungsberichte und Einblicke zu Kampagnen generieren. Guthaben wird basierend auf der Anzahl der Zeilen in Kampagnenberichten über alle Kampagnen hinweg und der Häufigkeit des Reportings genutzt, z. B. täglich, alle drei Tage oder wöchentlich.

## Kreditnutzung verwalten {#manage-credit-consumption}

So verwalten Sie Ihren Kreditverbrauch effektiv:

1. **Verstehen** den mit jeder Aktivität verbundenen Kreditverbrauch. Die [Collaboration-Produktbeschreibung](https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank} enthält eine Tabelle mit den Guthaben, die pro Aktivität verwendet werden.
2. **Nutzung regelmäßig überwachen**: Überprüfen Sie Ihre verfügbaren Credits und Aktivitätstabellen, um die Nutzungsmuster bei Audience-Management-, Audience-Zugriff-, Audience-Ausgangs- und Messaktivitäten zu verstehen.
3. **Nach Verbindung verfolgen**: Verwenden Sie den Verbindungsnamen, um zu ermitteln, welche Verbindungen die meisten Credits verbrauchen.
