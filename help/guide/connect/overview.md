---
title: Verbindungen – Überblick
description: Informationen zu Verbindungen in Real-Time CDP Collaboration.
audience: publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 5c08738cdc8e1e208203ee1f9a1cf1891b5b07cb
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 0%

---

# Verbindungen – Überblick

{{limited-availability-release-note}}

Bevor Mitwirkende an Kampagnen zusammenarbeiten können, müssen sie eine Verbindung herstellen. Diese Verbindung ermöglicht es ihnen, Zielgruppen zu aktivieren, Projekte zu erstellen und Berichte über die Kampagnenleistung zu erstellen.

Verbindungen werden basierend auf Ihrem ausgewählten Kooperationsmuster hergestellt. Collaboration unterstützt drei wichtige Zusammenarbeitsmuster: von Advertiser zu Publisher, von Marke zu Marke und von Advertiser zu Werbeplattform. Weitere Informationen zu diesen Mustern finden Sie im Handbuch [Kooperationsmuster](/help/guide/overview/collaboration-patterns.md) .

Um zu erfahren, wie Sie eine Verbindung herstellen, lesen Sie den folgenden Abschnitt, der Ihrem Kooperationsmuster entspricht:

- [Verbindung zwischen Advertiser und Publisher](#advertiser-to-publisher-connection)
- [Marke-zu-Marke-Verbindung](#brand-to-brand-connection)
- [Verbindung zwischen Werbekunden und Werbeplattform](#advertiser-to-advertising-platform-connection)

## Verbindung zwischen Advertiser und Publisher {#advertiser-to-publisher-connection}

![Allgemeine Abbildung des Verbindungsprozesses zwischen Advertiser und Publisher.](/help/assets/connect/establish-connection/advertiser-publisher-flow.png){zoomable="yes"}

Im Muster von Advertiser zu Publisher erkennt ein Advertiser einen Publisher, mit dem er arbeiten möchte, über den Arbeitsbereich **[!UICONTROL Discover Publishers]** und sendet eine Verbindungseinladung. Der Publisher prüft dann die Einladung und akzeptiert sie, sodass der Advertiser Verbindungseinstellungen vorschlagen kann. Sobald der Herausgeber die Verbindungseinstellungen akzeptiert, wird die Verbindung hergestellt und beide Mitarbeiter können mit der Arbeit an Projekten beginnen.

### Allgemeine Übersicht

Um eine Verbindung zwischen einem Advertiser und einem Publisher herzustellen, sind die folgenden Schritte erforderlich:

1. [Publisher entdecken](./discover-collaborators.md): Der Advertiser identifiziert potenzielle Publisher, mit denen er zusammenarbeiten soll.
2. [Einladung senden](./establishing-connections.md#send-invite): Der Advertiser sendet eine Einladung zur Verbindung an den ausgewählten Publisher.
3. [Einladung annehmen](./establishing-connections.md#accept-invite): Der Herausgeber prüft und akzeptiert die Einladung.
4. [Verbindungseinstellungen konfigurieren](./establishing-connections.md#configure-connection-settings): Der Advertiser konfiguriert die Verbindungseinstellungen und sendet sie zur Überprüfung an den Publisher.
5. [Verbindungseinstellungen bestätigen](./establishing-connections.md#review-connection-settings): Der Herausgeber prüft die Verbindungseinstellungen und akzeptiert oder lehnt sie ab. Wenn akzeptiert, wird die Verbindung hergestellt. Bei Ablehnung kann der Herausgeber Feedback für Revisionen außerhalb des Produkts geben. Der Werbetreibende kann dann die Einstellungen überarbeiten und zur Überprüfung erneut senden.

Sobald die Verbindungseinstellungen akzeptiert wurden, wird die Verbindung hergestellt und die Mitarbeiter können [&#x200B; Projekt erstellen](/help/guide/collaborate/manage-projects.md#create-project) um mit der Zusammenarbeit bei Kampagnen zu beginnen.

## Marke-zu-Marke-Verbindung {#brand-to-brand-connection}

![Allgemeine Abbildung des Verbindungsprozesses zwischen Marken.](/help/assets/connect/establish-connection/brand-to-brand-flow.png){zoomable="yes"}

>[!TIP]
>
>Der Begriff **Marke** wird verwendet, um ein Unternehmen oder eine Marke außerhalb von Collaboration zu bezeichnen. Der Begriff **Mitarbeiter** bezieht sich auf jedes Konto, das in Collaboration eine Verbindung herstellen kann, unabhängig davon, ob es sich um einen Advertiser oder einen Publisher handelt.

Im Marken-zu-Marken-Muster können sich zwei Marken, die außerhalb des Produkts kommuniziert haben, direkt in Collaboration über eine (private [) &#x200B;](#private-connection-invite) verbinden. Eine Marke kann entweder ein Advertiser oder ein Publisher sein. Dieses Muster ist besonders für Marken nützlich, die nicht zum herkömmlichen Advertiser-Publisher-Modell passen, z. B. zwei Advertiser oder zwei Publisher.

Zunächst sendet ein Mitarbeiter eine private Verbindungseinladung an einen anderen Mitarbeiter. Der Empfänger prüft die Einladung und akzeptiert sie, sodass der Besitzer Verbindungseinstellungen vorschlagen kann. Sobald der Empfänger die Verbindungseinstellungen akzeptiert, wird die Verbindung hergestellt und beide Mitarbeiter können mit der Arbeit an Projekten beginnen.

### Allgemeine Übersicht

>[!TIP]
>
>Bei der Erörterung des Verbindungsprozesses wird zwischen dem **Eigentümer** und dem **Empfänger** unterschieden. Der Eigentümer ist der Mitarbeiter, der die Verbindung initiiert, indem er die Einladung sendet, während der Empfänger der Mitarbeiter ist, der die Einladung empfängt und überprüft.

Der Verbindungsprozess zwischen zwei Marken umfasst mehrere Schritte. Bevor der Verbindungsprozess beginnt, müssen einige Voraussetzungen erfüllt sein:

1. Zwei Marken kommunizieren außerhalb des Produkts, um die potenzielle Verbindung zu besprechen.
1. Die Marken [erstellen &#x200B;](/help/guide/setup/onboard-account.md) in Collaboration, falls noch nicht geschehen, und achten darauf, den entsprechenden Rollentyp (Advertiser oder Publisher) auszuwählen.

Sobald die Voraussetzungen erfüllt sind, kann der Verbindungsprozess gestartet werden. Die folgenden Schritte beschreiben den Prozess:

1. [Einladung zur privaten Verbindung senden](./establishing-connections.md#private-connection-invite): Ein Mitarbeiter sendet eine Einladung zur privaten Verbindung an einen anderen Mitarbeiter.
2. [Einladung zur privaten Verbindung akzeptieren](./establishing-connections.md#accept-invite): Der Empfänger prüft und akzeptiert die Einladung zur privaten Verbindung.
3. [Verbindungseinstellungen konfigurieren](./establishing-connections.md#configure-connection-settings): Der Eigentümer konfiguriert die Verbindungseinstellungen und sendet sie zur Überprüfung und Annahme an den Empfänger.
4. [Verbindungseinstellungen bestätigen](./establishing-connections.md#review-connection-settings): Der Empfänger prüft die Verbindungseinstellungen und akzeptiert oder lehnt sie ab.

Sobald die Verbindungseinstellungen akzeptiert wurden, wird die Verbindung hergestellt und die Mitarbeiter können [&#x200B; Projekt erstellen](/help/guide/collaborate/manage-projects.md#create-project) um mit der Zusammenarbeit bei Kampagnen zu beginnen.

## Verbindung zwischen Werbekunden und Werbeplattform {#advertiser-to-advertising-platform-connection}

Der Verbindungsprozess zwischen Werbetreibenden und der Werbeplattform ermöglicht es Werbetreibenden, eine Verbindung zu Werbeplattformen von Drittanbietern wie Amazon Marketing Cloud (AMC) herzustellen, um ihre Marketing-Funktionen zu verbessern.

### Allgemeine Übersicht

Der Verbindungsprozess zwischen einem Werbetreibenden und einer Werbeplattform umfasst mehrere Schritte. Bevor der Verbindungsprozess beginnt, stellen Sie sicher, dass Sie über ein aktives Konto bei der Werbeplattform verfügen und für die Verwendung ihrer Dienste zugelassen sind. Die folgenden Schritte beschreiben den Verbindungsprozess:

1. [Werbeplattformen entdecken](./discover-collaborators.md): Der Werbetreibende identifiziert potenzielle Werbeplattformen, mit denen er zusammenarbeiten kann.
2. [Mit Werbeplattform verbinden](./advertising-platforms/overview.md#advertising-platforms-overview): Der Advertiser initiiert den Verbindungsprozess, indem er die Werbeplattform auswählt, mit der er eine Verbindung herstellen möchte, und befolgt die Aufforderungen zur Authentifizierung und Autorisierung der Verbindung.
