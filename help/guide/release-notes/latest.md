---
title: Aktuelle Versionshinweise zu Real-Time CDP Collaboration
description: Folgen Sie den neuesten Versionen für Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
source-git-commit: afe8560a12017c6b993f93cde8636288aa6e4991
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 2%

---

# Aktuelle Versionshinweise zu Real-Time CDP Collaboration

{{limited-availability-release-note}}

**Letzte Aktualisierung**: August 2025.

In diesen Versionshinweisen werden die in Adobe Real-Time CDP Collaboration veröffentlichten Funktionen beschrieben. Collaboration-Versionen basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen ungefähren monatlichen Veröffentlichungsintervall ermöglicht. Diese Versionshinweise werden häufig aktualisiert. Überprüfen Sie sie daher regelmäßig.

## August 2025 {#august-2025}

* Collaboration unterstützt jetzt die folgenden [Übereinstimmungsschlüssel](../setup/onboard-account.md#supported-match-keys):
   * Gehashte E-Mail
   * Hash-Telefonnummer
   * CRM-ID
   * Treue-ID
   * Gehashtes IPv4
   * AdFixus-ID
* In Collaboration sind jetzt mehrere Übereinstimmungsschlüssel verfügbar, mit denen Sie Ihre Zielgruppengröße erweitern und die Übereinstimmungsraten verbessern können. Beim Sourcing von Audiences, Herstellen von Verbindungen und Aktivieren von Audiences können mehrere Übereinstimmungsschlüssel verwendet werden. Weitere Informationen zur Verwendung mehrerer Übereinstimmungsschlüssel finden Sie in den Handbüchern [Einrichten von Übereinstimmungsschlüsseln](../setup/onboard-account.md) und [Sourcing-Zielgruppen](../setup/onboard-audiences.md#map-fields).

>[!IMPORTANT]
>
>Beim Aktivieren von Zielgruppen, für die mehrere Übereinstimmungsschlüssel verwendet werden, schlägt die gesamte Aktivierung fehl, wenn ein (oder mehrere) Übereinstimmungsschlüssel keine Überschneidungen aufweisen, keine Zielgruppen zählen oder unter den Schwellenwert fallen. Stellen Sie vor der Aktivierung sicher, dass sich Ihre Zielgruppen ausreichend überschneiden und der Mindestschwellenwert von 1.000 IDs für alle Übereinstimmungsschlüssel erreicht wird.

* Das Adobe Experience Platform-Ziel unterstützt jetzt das Aktivieren von Zielgruppen mit mehreren Übereinstimmungsschlüsseln. Darüber hinaus können Sie jetzt einen verknüpften Schlüssel verwenden, wenn Sie die Zuordnung Ihres Ziels konfigurieren, um anzugeben, welcher Übereinstimmungsschlüssel während der Aktivierung gesendet wird. Weitere Informationen finden Sie im [Experience Platform-Ziel](../destinations/experience-platform.md#linked-keys)-Handbuch.
* Mitwirkende können jetzt mehrere Zielgruppen gleichzeitig bearbeiten. Mit dem Tool zur Massenbearbeitung können Sie jetzt Zielgruppen-Metadaten, Verbindungszugriff, Namen, Beschreibungen und Kategorien für mehrere Zielgruppen bearbeiten. Weitere Informationen zum Bearbeiten von Zielgruppen finden Sie im Handbuch [Verwalten ](../setup/onboard-audiences.md#edit-audiences) Zielgruppen“.

## Juli 2025 {#july-2025}

Real-Time CDP Collaboration unterstützt jetzt die Zusammenarbeit zwischen Marken. Mitwirkende können jetzt Verbindungen herstellen, unabhängig davon, ob sie ein Advertiser oder ein Publisher sind. Dies ermöglicht flexiblere Kooperationsmöglichkeiten und Marken, die Daten und Erkenntnisse des jeweils anderen zu nutzen. Weitere Informationen zu den Unterschieden zwischen der Zusammenarbeit von Marke zu Marke und der Zusammenarbeit zwischen Advertiser und Publisher finden Sie im Handbuch [Collaboration Patterns](../overview/collaboration-patterns.md) .

* Mitwirkende können sich jetzt über „Einladungen zu privaten [&quot; miteinander ](../connect/establishing-connections.md#private-connection-invites). Geben Sie den eindeutigen Verbindungs-Code Ihres Kontos für einen Mitwirkenden frei, der ihn dann verwenden kann, um sich direkt mit Ihnen zu verbinden. Dies ist eine Kernfunktion der Zusammenarbeit zwischen Marken, die es Mitarbeitern ermöglicht, Verbindungen jenseits von Werbetreibenden herzustellen und das Verzeichnis **[!UICONTROL Discover Publishers]** zu erkunden.
* [Selbstbedienungsziele](../setup/manage-destinations.md) sind jetzt sowohl für Werbetreibende als auch für Herausgeber verfügbar.
* Die Zielgruppenaktivierung ist jetzt für beide Mitwirkenden in einer Verbindung verfügbar, unabhängig von ihrer [Kontorolle](../overview/roles.md). Die Einstellungen für die Zielgruppenaktivierung werden beim [Herstellen von Verbindungen](../connect/establishing-connections.md#configure-connection-settings) konfiguriert, sodass Sie angeben können, welcher Mitarbeiter Zielgruppen aktivieren kann. Weitere Informationen zur Aktivierung von Zielgruppen finden Sie im Handbuch [Aktivieren von Zielgruppen](../collaborate/activate.md).
* Der Anwendungsfall **[!UICONTROL Aktivieren]** wurde neu konfiguriert, um die Zusammenarbeit zwischen Marken zu unterstützen. Die **[!UICONTROL Aktivieren]**-Registerkarte innerhalb eines Projekts zeigt jetzt die Zielgruppen an, die an Ihren Mitarbeiter gesendet wurden, sowie die Zielgruppen, die von Ihrem Mitarbeiter für Ihr Ziel aktiviert wurden. Weitere Informationen finden Sie im Handbuch [Zielgruppen aktivieren](../collaborate/activate.md) . <br> ![Das Aktivierungs-Dashboard mit den Abschnitten „An Zielgruppen gesendet“ und „Aktivierte Zielgruppen“.](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* Audience-Indexwerte sind jetzt auf der Registerkarte **[!UICONTROL Entdecken]** eines Projekts verfügbar. Der Audience-Index-Wert ist ein Maß dafür, wie gut eine Zielgruppe mit der Zielgruppe Ihres Mitarbeiters übereinstimmt. Dieser Wert wird anhand der zugrunde liegenden Anzahl und Überschneidungen der Zielgruppen berechnet. Weitere Informationen zu Zielgruppenindex-Bewertungen finden Sie im Handbuch [Zielgruppenindex-Bewertung](../collaborate/discover.md#audience-index-score).

## Mai 2025 {#may-2025}

* Real-Time CDP Collaboration ist jetzt für Kunden in **Australien** und **Neuseeland** verfügbar. Sie ist für Kunden von Real-Time CDP Prime und Ultimate in diesen Regionen automatisch verfügbar.
* Real-Time CDP Collaboration bietet jetzt [Selbstbedienungsziele](../setup/manage-destinations.md) über die Registerkarte **[!UICONTROL Meine Ziele]** im Abschnitt **[!UICONTROL Setup]** an. Mit Zielen können Sie Zielgruppen in Drittanbieterplattformen wie Werbenetzwerken oder Datenverwaltungsplattformen aktivieren, um Ihre Kundinnen und Kunden über verschiedene Kanäle zu erreichen. Derzeit werden nur Adobe Experience Platform-Ziele unterstützt. Wenn Sie ein anderes Ziel konfigurieren möchten, wenden Sie sich an Ihren Adobe-Support-Mitarbeiter. Weitere Informationen zu Zielen finden Sie im Handbuch [Ziele - Übersicht](../destinations/overview.md) .
   * Ziele unterstützen auch die Anzeige von Collaboration-Zielgruppen im Zielgruppenportal [Adobe Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences).
* Sie können jetzt die Aktualisierungshäufigkeit der Zielgruppe für bestehende Datenverbindungen in Collaboration bearbeiten. Derzeit können Sie Ihre Zielgruppen täglich oder alle zwei bis sechs Tage aktualisieren. Weitere Informationen zum Bearbeiten der Aktualisierungshäufigkeit für Zielgruppen finden Sie im Handbuch [Datenverbindungen verwalten](../setup/manage-data-connection.md#scheduling).
* Für jeden innerhalb der Verbindung ausgewählten Anwendungsfall werden jetzt Credit-Splits zwischen Partnern festgelegt. Sie können für jeden Anwendungsfall unterschiedliche Regeln für den Kreditverbrauch festlegen, um die Verwendung Ihrer Gutschriften besser steuern zu können. Weitere Informationen zur Funktion der Kreditaufteilung finden Sie im Handbuch [Verbindungseinstellungen](../connect/establishing-connections.md#connection-settings) . Weitere Informationen zum Konsum von Guthaben finden Sie im Handbuch [Typen von ](../setup/my-activity.md#types-of-activities)). <br> ![Bildschirm mit den Verbindungseinstellungen mit der Funktion der Kreditaufteilung.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* Publisher können jetzt Advertiser-Namen und -IDs festlegen, bevor sie die Verbindungseinstellungen von einem Advertiser akzeptieren. Publisher können Namen und IDs festlegen, die mit ihren internen Systemen übereinstimmen, die sich von den Namen und IDs des Advertisers unterscheiden können. Weitere Informationen zum Hinzufügen von Advertiser-Namen und IDs finden Sie im Handbuch [Verbindungseinstellungen](../connect/establishing-connections.md#connection-settings.md) . <br> ![Bildschirm „Verbindungseinstellungen“ mit den Herausgebereinstellungen für Advertiser-Namen und -IDs.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## April 2025 {#april-2025}

* Die neue Spalte **[!UICONTROL Eingaben verarbeitet]** wurde der Aktivitätstabelle für Kreditverbrauch hinzugefügt. In dieser Spalte wird die Gesamtzahl der Eingaben (z. B. IDs oder Zeilen) angezeigt, die für jede Aktivität verarbeitet wurden. [Weitere Informationen](/help/guide/setup/my-activity.md#inputs-processed). <br> ![Spalte „Verarbeitete Eingaben“ in der Ansicht „Meine Aktivität“ hervorgehoben.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* Die neue Option Kontakt-E-Mail wurde zur Kontoerstellung hinzugefügt. Auf diese Weise können sich Partner-Mitarbeiter während des Verbindungsprozesses nach Bedarf mit Ihnen in Verbindung setzen. [Weitere Informationen](../setup/onboard-account.md).

## März 2025 {#march-2025}

* Beim [ von Zielgruppen ](/help/guide/setup/onboard-audiences.md) Collaboration können Sie jetzt eine Aktualisierungshäufigkeit für Zielgruppen von **alle ein bis sechs Tage)**, um die Kreditaktivität [Zielgruppenverwaltung“ besser zu ](/help/guide/setup/my-activity.md#types-of-activities). Weitere Informationen finden Sie im Handbuch [Verwalten ](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences) Zielgruppen“. <br> ![Bildschirm „Zeitplan“ mit verschiedenen Häufigkeitsintervallen zur Aktualisierung der Zielgruppenzugehörigkeit.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "Bildschirm „Zeitplan“ mit verschiedenen Häufigkeitsintervallen zur Aktualisierung der Zielgruppenzugehörigkeit."){width="250" align="center" zoomable="yes"}
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
* [End-to-End-Workflow](/help/guide/overview/end-to-end-workflow.md)
* [Berechtigungen - Übersicht](/help/guide/permissions/overview.md)
