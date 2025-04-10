---
title: Datenverbindungen verwalten
description: Erfahren Sie, wie Sie in Real-Time CDP Collaboration Datenverbindungen verwalten, einschließlich Übereinstimmungsschlüsseln, Planung, Anwendungsfällen und Zielgruppenfilterung
audience: administrator, data engineer
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 4%

---

# Datenverbindungen verwalten

{{limited-availability-release-note}}

## Überblick

Verwenden Sie Datenverbindungen in Real-Time CDP Collaboration, um Zielgruppen aus verschiedenen Quellen zu importieren. Erfahren Sie, wie Sie Übereinstimmungsschlüssel verwalten und Datenimporte für Ihre vorhandenen Datenverbindungen planen. Darüber hinaus können Sie Zielgruppen nach verschiedenen Attributen filtern, um detailliertere Einblicke zu erhalten.

Bevor Sie hier Ihre Datenverbindungen verwalten, sollten Sie sie zunächst während des Workflows [Zielgruppen-Onboarding](./onboard-audiences.md) einrichten. Dadurch wird sichergestellt, dass die richtigen Datenquellen für die Verwendung in Real-Time CDP Collaboration verbunden sind.

## Datenverbindungen anzeigen

>[!IMPORTANT]
>
>Das Löschen einer Datenverbindung wird derzeit in der Benutzeroberfläche von Real-Time CDP Collaboration nicht unterstützt. Um eine Datenverbindung zu löschen, wenden Sie sich an Ihren Adobe-Support-Mitarbeiter oder [erstellen Sie ein Support-Ticket](https://experienceleague.adobe.com/home?lang=en&amp;support-tab=open-ticket#support).

Um vorhandene Datenverbindungen anzuzeigen, navigieren Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Meine Zielgruppen]** und wählen Sie **[!UICONTROL Datenverbindungen verwalten]**.

![Arbeitsbereich „Setup“ mit hervorgehobener Option „Datenverbindungen verwalten“.](/help/assets/setup/manage-data-connection/manage-data-connection-highlighted.png)

Dadurch wird eine Ansicht aller Ihrer derzeit eingerichteten Datenverbindungen mit Informationen zur Anzahl der Zielgruppen in jeder dieser Verbindungen, zur Quelle der Datenverbindung und mehr angezeigt. Wählen Sie **[!UICONTROL Datenverbindung anzeigen]**, um Informationen über die Übereinstimmungsschlüssel, die Planung und die Zielgruppen anzuzeigen, die Teil dieser Datenverbindung sind.

![Arbeitsbereich „Datenverbindungen verwalten“ mit hervorgehobenen Optionen „Verbindungen anzeigen“. ](/help/assets/setup/manage-data-connection/view-data-connection-highlighted.png)

### Übereinstimmungsschlüssel {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="Übereinstimmungsschlüssel"
>abstract="Übereinstimmungsschlüssel bestimmen, wie Daten aus verschiedenen Quellen zugeordnet werden. Wählen Sie die Übereinstimmungsschlüssel aus, die für Ihre Anwendungsfälle und Datenschutzrichtlinien am relevantesten sind."

Übereinstimmungsschlüssel sind Kennungen, die zum Abgleichen von Mitgliedern über Zielgruppen hinweg aus verschiedenen Datenquellen hinweg verwendet werden. Zu den verfügbaren Übereinstimmungsschlüsseln gehören:

- **Hash-E-Mail**

Die in dieser Datenverbindung verwendeten Übereinstimmungsschlüssel können nicht bearbeitet werden.

![Ein Arbeitsbereich für Datenverbindungen mit hervorgehobenem Abschnitt „Übereinstimmungsschlüssel“.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png)

### Planung {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="Planung"
>abstract="Diese Ansicht zeigt die Planungsoptionen an, die Sie ursprünglich für Ihre Datenverbindung ausgewählt haben."

Sie können die Planungsoptionen, die Sie ursprünglich für Ihre Datenverbindung ausgewählt haben, nicht bearbeiten. Weitere Informationen zu den Planungsoptionen finden Sie [ Abschnitt „Planung](/help/guide/setup/onboard-audiences.md#schedule) im Dokument zum Audience-Import-Workflow.

![Ein Arbeitsbereich für Datenverbindungen mit hervorgehobenem Abschnitt „Planung“.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png)

## Verwalten von Zielgruppen {#manage-audiences}

In der Liste der Zielgruppen Ihrer Datenverbindung können Sie auswählen, ob Sie die Zielgruppen anzeigen, ihre Kategorien bearbeiten oder sie aus der Datenverbindung entfernen möchten.

![Ein Arbeitsbereich für Datenverbindungen mit hervorgehobenen Zielgruppen.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png)

## Nächste Schritte

Nach der Verwaltung Ihrer Datenverbindungen können Sie [Überschneidungen](/help/guide/collaborate/discover.md) zwischen Ihren Zielgruppen und den Zielgruppen entdecken, die Ihr Mitarbeiter entdeckt hat.
