---
title: Aktuelle Versionshinweise zu Real-Time CDP Collaboration
description: Folgen Sie den neuesten Versionen für Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
TQID: https://experienceleague.adobe.com/re4oFblCLiZpspWIS7D4EEYNh36EDhULEOd2-ccXH28
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: e6156a39107edb0e15e2115db0762f6a86801ed6
workflow-type: tm+mt
source-wordcount: 1968
ht-degree: 3%

---

# Aktuelle Versionshinweise zu Real-Time CDP Collaboration

{{limited-availability-release-note}}

**Letzte Aktualisierung**: Juli 2026.

In diesen Versionshinweisen werden die in Adobe Real-Time CDP Collaboration veröffentlichten Funktionen beschrieben. Collaboration-Versionen basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen ungefähren monatlichen Veröffentlichungsintervall ermöglicht. Diese Versionshinweise werden häufig aktualisiert. Überprüfen Sie sie daher regelmäßig.

## Juli 2026 {#july-2026}

Real-Time CDP Collaboration unterstützt jetzt zusätzliche Self-Service-Optionen zur Zielgruppenbeschaffung.

**Neue oder aktualisierte Funktionen**

| Funktion | Beschreibung |
| ------- | ----------- |
| Self-Service-Zielgruppenbeschaffung aus [!DNL Databricks Delta Share] und Adobe Audience Manager | Sie können jetzt Erstanbieter-Zielgruppen direkt aus Ihrer [!DNL Databricks Delta Share] beziehen oder geeignete Adobe Audience Manager-Segmente in Collaboration importieren. Anweisungen zum Einrichten finden Sie in den folgenden Handbüchern: <ul><li>[Konfigurieren [!DNL Databricks Delta Share]  für Zielgruppen-Sourcing](../setup/configure-databricks-audience-sourcing.md)</li><li>[Konfigurieren von Adobe Audience Manager für die Zielgruppen-Beschaffung](../setup/configure-aam-audience-sourcing.md)</li></ul> |

{style="table-layout:auto"}

## April 2026 {#april-2026}

Neue Funktionen sind jetzt in Real-Time CDP Collaboration verfügbar. Dazu gehören Collaboration-[!DNL Starter] für einladende Partner, erweiterte Zielgruppen-Beschaffung aus [!DNL Snowflake] und [!DNL Google Cloud Storage], Unterstützung für [!DNL Demdex ID (ECID)] als Übereinstimmungsschlüssel und zwei neue Mitwirkungspflichten: Agentur und Datenpartner.

**Neue oder aktualisierte Funktionen**

| Funktion | Beschreibung |
| ------- | ----------- |
| Real-Time CDP Collaboration [!DNL Starter] | Sie können jetzt Partner, die keine Collaboration-Lizenz haben, über Collaboration [!DNL Starter] zur Zusammenarbeit mit Ihnen einladen. Eingeladene Partner können innerhalb der freigegebenen Verbindung Zielgruppen beziehen, Überschneidungen erkennen und Zielgruppen aktivieren. Siehe [Collaboration [!DNL Starter] Übersicht](../overview/starter-overview.md), um zu beginnen. |
| Self-Service-Zielgruppenbeschaffung aus [!DNL Snowflake] und [!DNL Google Cloud Storage] | Sie können jetzt Erstanbieter-Zielgruppen direkt aus Ihrem [!DNL Snowflake Secure Data Share] oder [!DNL Google Cloud Storage] Bucket in Collaboration beziehen. Anweisungen zum Einrichten finden Sie in den folgenden Handbüchern: <ul><li>[Konfigurieren [!DNL Snowflake]  für Zielgruppen-Sourcing](../setup/configure-snowflake-audience-sourcing.md) </li><li> [Konfigurieren [!DNL Google Cloud Storage]  für Zielgruppen-Sourcing](../setup/configure-gcs-audience-sourcing.md) </li></ul> |
| Übereinstimmungsschlüssel [!DNL Demdex ID] | [!DNL Demdex ID] (ECID) wird jetzt als Übereinstimmungsschlüssel für die plattformübergreifende Zuordnung anonymer Cookie-basierter Identitäten unterstützt. Dadurch wird die Genauigkeit der Zielgruppenüberschneidung verbessert, ohne auf authentifizierte Benutzerdaten angewiesen zu sein. Siehe [Unterstützte Übereinstimmungsschlüssel](../setup/onboard-account.md#supported-match-keys) für Details. |
| Neue Mitarbeiter-Rollen | Collaboration unterstützt jetzt zwei zusätzliche Rollen als Mitwirkende, einschließlich **Agency** und **Data Partner**. Durch diese Rollen wird erweitert, wie verschiedene Organisationen innerhalb der Plattform teilnehmen und zusammenarbeiten können. Weitere Informationen: <ul><li>[Rollen für Mitarbeiter-Konten](../overview/roles.md)</li><li>[Collaboration-Muster](../overview/collaboration-patterns.md)</li><li>[End-to-End-Workflow](../overview/end-to-end-workflow.md)</li></ul> |

{style="table-layout:auto"}

## März 2026 {#march-2026}

Sie können jetzt in Real-Time CDP Collaboration Messberichte für Kampagnen generieren und Messdaten verwalten.

**Neue oder aktualisierte Funktionen**

| Funktion | Beschreibung |
| ------- | ----------- |
| Allgemeine Verfügbarkeit der Messung | Messberichte sind jetzt in Collaboration allgemein verfügbar. Sie können jetzt mit Marketing-Kampagnen verknüpfte Kampagnen-IDs als Publisher eingeben, Konversionsdaten als Advertiser abrufen und zwei Berichtstypen generieren: **Kampagnenübersicht** für die gesamten Kampagnenergebnisse und **Attribution** für Einblicke in die Kampagnenwirksamkeit. Informationen zu den ersten Schritten finden Sie in den folgenden Handbüchern: <ul><li>[Kampagnen-IDs eingeben](../collaborate/manage-projects.md#manage-campaign-id)</li><li>[Source-Konversionsdaten](../setup/onboard-measurement-data.md)</li><li>[Erstellen und Anzeigen von Messberichten](../collaborate/measure.md)</li></ul> |
| Verwaltung des Messzyklus | Collaboration unterstützt auch die Messverwaltung:<ul><li> Werbetreibende können jetzt sowohl Messdatenverbindungen als auch zugehörige Konversionsereignisse bearbeiten oder löschen, um eine genaue und aktuelle Kampagnenanalyse zu gewährleisten. Weitere Informationen finden Sie unter [Verwalten der Messdatenverbindung](../setup/manage-measurement-data-connection.md) und [Verwalten von Konversionsereignissen](../setup/onboard-measurement-data.md#edit-measurement-data).</li><li>Sie können geplante Messberichte auch direkt über die Registerkarte **[!UICONTROL Kennzahlen]** in jedem beliebigen Kooperationsprojekt bearbeiten oder löschen. Dies steht allen Benutzern zur Verfügung. Weitere Einzelheiten finden Sie [&#x200B; Handbuch &#x200B;](../collaborate/measure.md) Verwalten von Messberichten .</li></ul> |

{style="table-layout:auto"}

## Februar 2026 {#february-2026}

Real-Time CDP Collaboration unterstützt jetzt die direkte Bearbeitung vorhandener Verbindungs- und Datenverbindungseinstellungen in der -Benutzeroberfläche.

**Neue oder aktualisierte Funktion**

| Funktion | Beschreibung |
| ------- | ----------- |
| Verbindungseinstellungen bearbeiten | Verbindungsbesitzer können jetzt Anwendungsfälle, Übereinstimmungsschlüssel, Aktivierungsberechtigungen und Kreditaufteilungen aktualisieren, nachdem eine Verbindung hergestellt wurde. Eine [&#x200B; Anleitung finden &#x200B;](../connect/manage-connections.md#edit-connection) unter „Bearbeiten einer Verbindung“. |
| Datenverbindungen bearbeiten | Aktualisieren Sie Übereinstimmungsschlüssel und Planungskonfigurationen für Ihre vorhandenen Datenverbindungen direkt in Collaboration. Eine [&#x200B; Anleitung finden Sie unter &#x200B;](../setup/manage-data-connection.md#edit-data-connection) von Datenverbindungen bearbeiten . |

## Januar 2026 {#january-2026}

Real-Time CDP Collaboration unterstützt jetzt den CSV-Datei-Upload als neue Methode zur Beschaffung von Zielgruppen sowie neue mobile Übereinstimmungsschlüssel (IDFA und GAID) für einen verbesserten Zielgruppenabgleich und eine verbesserte Messung.

**Neue oder aktualisierte Funktionen**

| Funktion | Beschreibung |
| ------- | ----------- |
| CSV-Upload für Zielgruppen-Sourcing | Laden Sie CSV-Dateien direkt über die Benutzeroberfläche in Collaboration in die Quell-Audiences hoch. Ideal für das Onboarding von First-Party-Daten für kurzfristige Kooperationsprojekte. Weitere Informationen finden Sie im [CSV-Datei für Zielgruppen-Sourcing hochladen](../setup/upload-csv-audience-sourcing.md). |
| Unterstützung für Mobile Match-Schlüssel | Collaboration unterstützt jetzt mobile Übereinstimmungsschlüssel, einschließlich IDFA und GAID, zum Abgleichen und Messen von Zielgruppen. Diese Übereinstimmungsschlüssel werden während der Kontoeinrichtung ausgewählt und können dann bei der Konfiguration der Verbindungseinstellungen für neue Verbindungen und in nachgelagerten Kollaborations-Workflows verwendet werden. Weitere Einzelheiten finden Sie [&#x200B; „Einrichtungshandbuch &#x200B;](../setup/onboard-account.md#set-up-match-keys) Übereinstimmungsschlüssel“. |

{style="table-layout:auto"}

## Dezember 2025 {#december-2025}

Real-Time CDP Collaboration ist jetzt für Kunden in **Europa, dem Nahen Osten und Afrika (EMEA)) verfügbar**. Sie ist für Kunden von Real-Time CDP Prime und Ultimate in diesen Regionen automatisch verfügbar.

## August 2025 {#august-2025}

Real-Time CDP Collaboration ist jetzt für Kunden in **Kanada** verfügbar. Sie ist für Kunden von Real-Time CDP Prime und Ultimate in diesen Regionen automatisch verfügbar.

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
>Beim Aktivieren von Zielgruppen, für die mehrere Übereinstimmungsschlüssel verwendet werden, schlägt die gesamte Aktivierung fehl, wenn ein (oder mehrere) Übereinstimmungsschlüssel keine Überschneidungen, keine Zielgruppengröße oder einen Schwellenwert unterschreiten. Stellen Sie vor der Aktivierung sicher, dass sich Ihre Zielgruppen ausreichend überschneiden und der Mindestschwellenwert von 1.000 IDs für alle Übereinstimmungsschlüssel erreicht wird.

* Das Adobe Experience Platform-Ziel unterstützt jetzt das Aktivieren von Zielgruppen mit mehreren Übereinstimmungsschlüsseln. Darüber hinaus können Sie jetzt einen verknüpften Schlüssel verwenden, wenn Sie die Zuordnung Ihres Ziels konfigurieren, um anzugeben, welcher Übereinstimmungsschlüssel während der Aktivierung gesendet wird. Weitere Informationen finden Sie im [Experience Platform-Ziel](../destinations/experience-platform.md#linked-keys)-Handbuch.
* Mitwirkende können jetzt mehrere Zielgruppen gleichzeitig bearbeiten. Mit dem Tool zur Massenbearbeitung können Sie jetzt Zielgruppen-Metadaten, Verbindungszugriff, Namen, Beschreibungen und Kategorien für mehrere Zielgruppen bearbeiten. Weitere Informationen zum Bearbeiten von Zielgruppen finden Sie im Handbuch [Verwalten &#x200B;](../setup/onboard-audiences.md#edit-audiences) Zielgruppen“.

## Juli 2025 {#july-2025}

Real-Time CDP Collaboration unterstützt jetzt die Zusammenarbeit zwischen Marken. Mitwirkende können jetzt Verbindungen herstellen, unabhängig davon, ob sie ein Advertiser oder ein Publisher sind. Dies ermöglicht flexiblere Kooperationsmöglichkeiten und Marken, die Daten und Erkenntnisse des jeweils anderen zu nutzen. Weitere Informationen zu den Unterschieden zwischen der Zusammenarbeit von Marke zu Marke und der Zusammenarbeit zwischen Advertiser und Publisher finden Sie im Handbuch [Collaboration Patterns](../overview/collaboration-patterns.md) .

* Mitwirkende können sich jetzt über „Einladungen zu privaten [&quot; miteinander &#x200B;](../connect/establishing-connections.md#private-connection-invites). Geben Sie den eindeutigen Verbindungs-Code Ihres Kontos für einen Mitwirkenden frei, der ihn dann verwenden kann, um sich direkt mit Ihnen zu verbinden. Dies ist eine Kernfunktion der Zusammenarbeit zwischen Marken, die es Mitarbeitern ermöglicht, Verbindungen jenseits von Werbetreibenden herzustellen, die das Verzeichnis **[!UICONTROL Discover Collaborators]** durchsuchen.
* [Selbstbedienungsziele](../setup/manage-destinations.md) sind jetzt sowohl für Werbetreibende als auch für Herausgeber verfügbar.
* Die Zielgruppenaktivierung ist jetzt für beide Mitwirkenden in einer Verbindung verfügbar, unabhängig von ihrer [Kontorolle](../overview/roles.md). Die Einstellungen für die Zielgruppenaktivierung werden beim [Herstellen von Verbindungen](../connect/establishing-connections.md#configure-connection-settings) konfiguriert, sodass Sie angeben können, welcher Mitarbeiter Zielgruppen aktivieren kann. Weitere Informationen zur Aktivierung von Zielgruppen finden Sie im Handbuch [Aktivieren von Zielgruppen](../collaborate/activate.md).
* Der Anwendungsfall **[!UICONTROL Aktivieren]** wurde neu konfiguriert, um die Zusammenarbeit zwischen Marken zu unterstützen. Die **[!UICONTROL Aktivieren]**-Registerkarte innerhalb eines Projekts zeigt jetzt die Zielgruppen an, die an Ihren Mitarbeiter gesendet wurden, sowie die Zielgruppen, die von Ihrem Mitarbeiter für Ihr Ziel aktiviert wurden. Weitere Informationen finden Sie im Handbuch [Zielgruppen aktivieren](../collaborate/activate.md) . <br> ![Das Aktivierungs-Dashboard mit den Abschnitten „An Zielgruppen gesendet“ und „Aktivierte Zielgruppen“.](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* Audience-Indexwerte sind jetzt auf der Registerkarte **[!UICONTROL Entdecken]** eines Projekts verfügbar. Der Audience-Index-Wert ist ein Maß dafür, wie gut eine Zielgruppe mit der Zielgruppe Ihres Mitarbeiters übereinstimmt. Dieser Wert wird anhand der zugrunde liegenden Zielgruppengröße und Überschneidungen berechnet. Weitere Informationen zu Zielgruppenindex-Bewertungen finden Sie im Handbuch [Zielgruppenindex-Bewertung](../collaborate/discover.md#audience-index-score).

## Mai 2025 {#may-2025}

* Real-Time CDP Collaboration ist jetzt für Kunden in **Australien** und **Neuseeland** verfügbar. Sie ist für Kunden von Real-Time CDP Prime und Ultimate in diesen Regionen automatisch verfügbar.
* Real-Time CDP Collaboration bietet jetzt [Selbstbedienungsziele](../setup/manage-destinations.md) über die Registerkarte **[!UICONTROL Meine Ziele]** im Abschnitt **[!UICONTROL Setup]** an. Mit Zielen können Sie Zielgruppen in Drittanbieterplattformen wie Werbenetzwerken oder Datenverwaltungsplattformen aktivieren, um Ihre Kundinnen und Kunden über verschiedene Kanäle zu erreichen. Derzeit werden nur Adobe Experience Platform-Ziele unterstützt. Wenn Sie ein anderes Ziel konfigurieren möchten, wenden Sie sich an Ihren Adobe-Support-Mitarbeiter. Weitere Informationen zu Zielen finden Sie im Handbuch [Ziele - Übersicht](../destinations/overview.md) .
  * Ziele unterstützen auch die Anzeige von Collaboration-Zielgruppen im Zielgruppenportal [Adobe Experience Platform](https://experienceleague.adobe.com/de/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences).
* Sie können jetzt die Aktualisierungshäufigkeit der Zielgruppe für bestehende Datenverbindungen in Collaboration bearbeiten. Derzeit können Sie Ihre Zielgruppen täglich oder alle zwei bis sechs Tage aktualisieren. Weitere Informationen zum Bearbeiten der Aktualisierungshäufigkeit für Zielgruppen finden Sie im Handbuch [Datenverbindungen verwalten](../setup/manage-data-connection.md#scheduling).
* Für jeden innerhalb der Verbindung ausgewählten Anwendungsfall werden jetzt Credit-Splits zwischen Partnern festgelegt. Sie können für jeden Anwendungsfall unterschiedliche Regeln für den Kreditverbrauch festlegen, um die Verwendung Ihrer Gutschriften besser steuern zu können. Weitere Informationen zur Funktion der Kreditaufteilung finden Sie im Handbuch [Verbindungseinstellungen](../connect/establishing-connections.md#connection-settings) . Weitere Informationen zum Konsum von Guthaben finden Sie im Handbuch [Typen von &#x200B;](../setup/my-activity.md#types-of-activities)). <br> ![Bildschirm mit den Verbindungseinstellungen mit der Funktion der Kreditaufteilung.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* Publisher können jetzt Advertiser-Namen und -IDs festlegen, bevor sie die Verbindungseinstellungen von einem Advertiser akzeptieren. Publisher können Namen und IDs festlegen, die mit ihren internen Systemen übereinstimmen, die sich von den Namen und IDs des Advertisers unterscheiden können. Weitere Informationen zum Hinzufügen von Advertiser-Namen und IDs finden Sie im Handbuch [Verbindungseinstellungen](../connect/establishing-connections.md#connection-settings.md) . <br> ![Bildschirm „Verbindungseinstellungen“ mit den Herausgebereinstellungen für Advertiser-Namen und -IDs.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## April 2025 {#april-2025}

* Die neue Spalte **[!UICONTROL Eingaben verarbeitet]** wurde der Aktivitätstabelle für Kreditverbrauch hinzugefügt. In dieser Spalte wird die Gesamtzahl der Eingaben (z. B. IDs oder Zeilen) angezeigt, die für jede Aktivität verarbeitet wurden. [Weitere Informationen](/help/guide/setup/my-activity.md#inputs-processed). <br> ![Spalte „Verarbeitete Eingaben“ in der Ansicht „Meine Aktivität“ hervorgehoben.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* Die neue Option Kontakt-E-Mail wurde zur Kontoerstellung hinzugefügt. Auf diese Weise können sich Partner-Mitarbeiter während des Verbindungsprozesses nach Bedarf mit Ihnen in Verbindung setzen. [Weitere Informationen](../setup/onboard-account.md).

## März 2025 {#march-2025}

* Beim [&#x200B; von Zielgruppen &#x200B;](/help/guide/setup/onboard-audiences.md) Collaboration können Sie jetzt eine Aktualisierungshäufigkeit für Zielgruppen von **alle ein bis sechs Tage)**, um die Kreditaktivität [Zielgruppenverwaltung“ besser zu &#x200B;](/help/guide/setup/my-activity.md#types-of-activities). Weitere Informationen finden Sie im Handbuch [Verwalten &#x200B;](https://experienceleague.adobe.com/de/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences) Zielgruppen“. <br> ![Bildschirm „Zeitplan“ mit verschiedenen Häufigkeitsintervallen zur Aktualisierung der Zielgruppenzugehörigkeit.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "Bildschirm „Zeitplan“ mit verschiedenen Häufigkeitsintervallen zur Aktualisierung der Zielgruppenzugehörigkeit."){width="250" align="center" zoomable="yes"}
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
3. **Verbindungen herstellen**: Beginn der Zusammenarbeit mit vertrauenswürdigen Werbetreibenden oder Publishern. Weitere Informationen zum Herstellen von Verbindungen finden Sie im [&#x200B; zum Herstellen von Verbindungen &#x200B;](/help/guide/connect/establishing-connections.md).
4. **Discover &amp; Activate**: Erstellen Sie Projekte, um wertvolle Zielgruppen zu identifizieren, die in Kampagnen aktiviert werden sollen. Weitere Informationen zum Erstellen von Projekten finden Sie im Handbuch [Verwalten &#x200B;](/help/guide/collaborate/manage-projects.md) Projekten“.

### Verfügbarkeit

* Adobe Real-Time CDP Collaboration ist derzeit nur für Kunden aus den USA verfügbar.
* Sie ist automatisch für Kunden von Adobe Real-Time CDP Prime und Ultimate verfügbar

Weitere Informationen finden Sie im Abschnitt:

* [Übersicht über Collaboration](/help/guide/home.md)
* [End-to-End-Workflow](/help/guide/overview/end-to-end-workflow.md)
* [Berechtigungen - Übersicht](/help/guide/permissions/overview.md)
