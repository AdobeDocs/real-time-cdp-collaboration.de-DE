---
title: Aktuelle Versionshinweise zu Real-Time CDP Collaboration
description: Folgen Sie den neuesten Versionen für Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 2%

---

# Aktuelle Versionshinweise zu Real-Time CDP Collaboration

{{limited-availability-release-note}}

**Letzte Aktualisierung**: Mai 2025.

In diesen Versionshinweisen werden die in Adobe Real-Time CDP Collaboration veröffentlichten Funktionen beschrieben. Collaboration-Versionen basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen ungefähren monatlichen Veröffentlichungsintervall ermöglicht. Diese Versionshinweise werden häufig aktualisiert. Überprüfen Sie sie daher regelmäßig.

## Mai 2025 {#may-2025}

* Real-Time CDP Collaboration ist jetzt für Kunden in **Australien** und **Neuseeland** verfügbar. Sie ist für Kunden von Real-Time CDP Prime und Ultimate in diesen Regionen automatisch verfügbar.
* Real-Time CDP Collaboration bietet jetzt [Selbstbedienungsziele](../setup/manage-destinations.md) über die Registerkarte **[!UICONTROL Meine Ziele]** im Abschnitt **[!UICONTROL Setup]** an. Mit Zielen können Sie Zielgruppen in Drittanbieterplattformen wie Werbenetzwerken oder Datenverwaltungsplattformen aktivieren, um Ihre Kundinnen und Kunden über verschiedene Kanäle zu erreichen. Derzeit werden nur Adobe Experience Platform-Ziele unterstützt. Wenn Sie ein anderes Ziel konfigurieren möchten, wenden Sie sich an Ihren Adobe-Support-Mitarbeiter. Weitere Informationen zu Zielen finden Sie im Handbuch [Ziele - Übersicht](../destinations/overview.md) .
   * Ziele unterstützen auch die Anzeige von Collaboration-Zielgruppen im Zielgruppenportal [Adobe Experience Platform](https://experienceleague.adobe.com/de/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences).
* Sie können jetzt die Aktualisierungshäufigkeit der Zielgruppe für bestehende Datenverbindungen in Collaboration bearbeiten. Derzeit können Sie Ihre Zielgruppen täglich oder alle zwei bis sechs Tage aktualisieren. Weitere Informationen zum Bearbeiten der Aktualisierungshäufigkeit für Zielgruppen finden Sie im Handbuch [Datenverbindungen verwalten](../setup/manage-data-connection.md#scheduling).
* Für jeden innerhalb der Verbindung ausgewählten Anwendungsfall werden jetzt Credit-Splits zwischen Partnern festgelegt. Sie können für jeden Anwendungsfall unterschiedliche Regeln für den Kreditverbrauch festlegen, um die Verwendung Ihrer Gutschriften besser steuern zu können. Weitere Informationen zur Funktion der Kreditaufteilung finden Sie im Handbuch [Verbindungseinstellungen](../connect/establishing-connections.md#connection-settings) . Weitere Informationen zum Konsum von Guthaben finden Sie im Handbuch [Typen von ](../setup/my-activity.md#types-of-activities)). <br> ![Bildschirm mit den Verbindungseinstellungen mit der Funktion der Kreditaufteilung.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* Publisher können jetzt Advertiser-Namen und -IDs festlegen, bevor sie die Verbindungseinstellungen von einem Advertiser akzeptieren. Publisher können Namen und IDs festlegen, die mit ihren internen Systemen übereinstimmen, die sich von den Namen und IDs des Advertisers unterscheiden können. Weitere Informationen zum Hinzufügen von Advertiser-Namen und IDs finden Sie im Handbuch [Verbindungseinstellungen](../connect/establishing-connections.md#connection-settings.md) . <br> ![Bildschirm „Verbindungseinstellungen“ mit den Herausgebereinstellungen für Advertiser-Namen und -IDs.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## April 2025 {#april-2025}

* Die neue Spalte **[!UICONTROL Eingaben verarbeitet]** wurde der Aktivitätstabelle für Kreditverbrauch hinzugefügt. In dieser Spalte wird die Gesamtzahl der Eingaben (z. B. IDs oder Zeilen) angezeigt, die für jede Aktivität verarbeitet wurden. [Weitere Informationen](/help/guide/setup/my-activity.md#inputs-processed). <br> ![Spalte „Verarbeitete Eingaben“ in der Ansicht „Meine Aktivität“ hervorgehoben.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* Die neue Option Kontakt-E-Mail wurde zur Kontoerstellung hinzugefügt. Auf diese Weise können sich Partner-Mitarbeiter während des Verbindungsprozesses nach Bedarf mit Ihnen in Verbindung setzen. [Weitere Informationen](../setup/onboard-account.md).

## März 2025 {#march-2025}

* Beim [ von Zielgruppen ](/help/guide/setup/onboard-audiences.md) Collaboration können Sie jetzt eine Aktualisierungshäufigkeit für Zielgruppen von **alle ein bis sechs Tage)**, um die Kreditaktivität [Zielgruppenverwaltung“ besser zu ](/help/guide/setup/my-activity.md#types-of-activities). Weitere Informationen finden Sie im Handbuch [Verwalten ](https://experienceleague.adobe.com/de/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences) Zielgruppen“. <br> ![Bildschirm „Zeitplan“ mit verschiedenen Häufigkeitsintervallen zur Aktualisierung der Zielgruppenzugehörigkeit.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "Bildschirm „Zeitplan“ mit verschiedenen Häufigkeitsintervallen zur Aktualisierung der Zielgruppenzugehörigkeit."){width="250" align="center" zoomable="yes"}
* Beim Herstellen einer Verbindung mit einem Mitarbeiter können Sie jetzt aus vordefinierten **Anwendungsfällen** auswählen. Der ausgewählte Anwendungsfall bestimmt, welche Projektabschnitte und Produktfunktionen verfügbar werden. Weitere Informationen finden Sie im Handbuch [Verwalten von Projekten](/help/guide/collaborate/manage-projects.md#project-use-cases).
   * *Messung* aktiviert den Projektabschnitt **Messen**.
   * *Zielgruppenerkennung* aktiviert den Projektabschnitt **Entdecken**.
   * *Zielgruppenaktivierung* aktiviert die **Aktivieren**-Projektabschnitte <br>
* Sie können jetzt Verbindungen mit Mitarbeitern löschen, mit denen Sie nicht mehr arbeiten möchten. Informationen zum Löschen von Verbindungen finden Sie im Handbuch [Löschen von Verbindungen](/help/guide/connect/establishing-connections.md#delete-connections) .

## Februar 2025 {#february-2025}

Adobe Real-Time CDP Collaboration wurde entwickelt, um es Werbetreibenden und Publishern zu ermöglichen, hochwertige Zielgruppen ohne Drittanbieter-Cookies zu entdecken, zu aktivieren und zu messen, und ist jetzt in den Vereinigten Staaten allgemein verfügbar.

### Erste Schritte

1. **Zugriffseinrichtung**: Systemadministratoren konfigurieren Zugriffsberechtigungen für Benutzer. Weitere Informationen zum Konfigurieren von Zugriffsberechtigungen finden Sie im [Verwalten des Benutzerzugriffs](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access).
2. **Verbinden von Datenquellen**: Source-Zielgruppen zur Verwendung in Collaboration. Um mit der Beschaffung von Zielgruppen zu beginnen, lesen Sie das Handbuch [Quelle und Zielgruppen verwalten](/help/guide/setup/onboard-audiences.md).
3. **Verbindungen herstellen**: Beginn der Zusammenarbeit mit vertrauenswürdigen Werbetreibenden oder Publishern. Weitere Informationen zum Herstellen von Verbindungen finden Sie im [ zum Herstellen von Verbindungen ](/help/guide/connect/establishing-connections.md).
4. **Discover &amp; Activate**: Erstellen Sie Projekte, um wertvolle Zielgruppen zu identifizieren, die in Kampagnen aktiviert werden sollen. Weitere Informationen zum Erstellen von Projekten finden Sie im Handbuch [Verwalten ](/help/guide/collaborate/manage-projects.md) Projekten“.

### Verfügbarkeit

* Adobe Real-Time CDP Collaboration ist derzeit nur für Kunden aus den USA verfügbar.
* Sie ist automatisch für Kunden von Adobe Real-Time CDP Prime und Ultimate verfügbar

Weitere Informationen finden Sie im Abschnitt:

* [Übersicht über Collaboration](/help/guide/home.md)
* [End-to-End-Workflow](/help/guide/end-to-end-workflow.md)
* [Berechtigungen - Übersicht](/help/guide/permissions/overview.md)
