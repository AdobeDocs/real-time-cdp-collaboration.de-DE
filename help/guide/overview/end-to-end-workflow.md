---
title: End-to-End-Workflow
description: Machen Sie sich mit dem End-to-End-Workflow der Verwendung von Real-Time CDP Collaboration auf der Grundlage Ihres Kooperationsmusters vertraut.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
source-git-commit: 901b17c7493e76b17e780b6f7b05a69fa22303d2
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 0%

---

# End-to-End-Workflow

{{limited-availability-release-note}}

In Adobe Real-Time CDP Collaboration variiert der End-to-End-Workflow je nach ausgewähltem Zusammenarbeitsmuster. Der Workflow beschreibt die Schritte, die bei der Einrichtung und Ausführung eines Collaboration-Projekts erforderlich sind, von der Erstellung von Konten und der Beschaffung von Zielgruppen bis hin zur Herstellung von Verbindungen und zur Erstellung von Projekten. Das Verständnis dieses Workflows ist von entscheidender Bedeutung, um die Funktionen der Plattform effektiv nutzen zu können, um Ihre Marketing-Ziele zu erreichen.

## Erste Schritte

Bevor Sie beginnen, stellen Sie sicher, dass Sie über ein solides Verständnis dieser Schlüsselkonzepte verfügen:

- **Collaboration-Muster**: Diese Muster definieren, wie Kollaborateure zusammenarbeiten. Es gibt fünf verschiedene Muster:
   - [Advertiser-zu-Publisher](./collaboration-patterns.md#advertiser-to-publisher)
   - [Marke-zu-Marke](./collaboration-patterns.md#brand-to-brand)
   - [Advertiser-to-Data-Partner](./collaboration-patterns.md#advertiser-to-data-partner)
   - [Agentur-Verlag](./collaboration-patterns.md#agency-to-publisher)
   - [Advertiser-to-Agency-Plattform](./collaboration-patterns.md#advertiser-to-agency-platform)
- **Kontorollen**: Kontorollen bestimmen Ihre Funktionen innerhalb der Plattform. Sie sollten mit den Zielen, der Marke und den Zielen Ihres Unternehmens übereinstimmen. Es gibt vier Kontorollen: [Advertiser](./roles.md#advertiser), [Publisher](./roles.md#publisher), [Agency](./roles.md#agency) und [data partner](./roles.md#data-partner).
- **Anwendungsfälle**: Anwendungsfälle definieren, wie Sie Collaboration zum Erreichen Ihrer Marketing-Ziele nutzen können. Es gibt drei Anwendungsfälle für die Zusammenarbeit: [Entdecken](./use-cases.md#discover), [Aktivieren](./use-cases.md#activate) und [Messen](./use-cases.md#measure).

In diesem Handbuch werden drei Pseudo-Kollaborateure verwendet, um den End-to-End-Workflow zu veranschaulichen:

- **[!UICONTROL Luma]**: Eine Sportbekleidungsmarke. Sie sind ein Advertiser, der durch zielgerichtete Marketing-Kampagnen bestimmte Zielgruppen erreichen möchte.
- **[!UICONTROL TV Tube]**: Ein digitaler Streaming-Anbieter. Sie sind ein Publisher, der Zielgruppendaten für die Verwendung durch Advertiser bereitstellt.
- **[!UICONTROL Fit Apparel]**: Eine weitere Sportbekleidungsmarke. Sie sind ein zweiter Werbetreibender, der zusammenarbeiten möchte, um Zielgruppendaten und Einblicke für verbesserte Marketing-Maßnahmen zu teilen.
- **[!UICONTROL Agency99]**: Eine Medienagentur. Sie verwalten mehrere Kundenkonten in ihrem Arbeitsbereich und stellen Verbindungen zu Publishern und Advertisern her.
- **[!UICONTROL DataM8]**: ein Drittanbieter von Daten. Sie stellen Zielgruppendaten zur Verwendung durch Werbetreibende bereit.
- **[!UICONTROL Holdco]**: eine Agentur-Holding-Plattform für Marketing- und Werbedienstleistungen, die von internen Agenturteams zur Verwaltung von Kundenkampagnen verwendet wird.

## Workflow von Advertiser zu Publisher {#advertiser-to-publisher-workflow}

[!UICONTROL Luma], ein Sporteinzelhandelsunternehmen, möchte eine Verbindung mit [!UICONTROL TV Tube], einem digitalen Streaming-Anbieter, herstellen, um bestimmte Zielgruppen durch zielgerichtete Marketing-Kampagnen zu erreichen.

Zunächst muss [!UICONTROL Luma] mit der Advertiser[&#128279;](../setup/onboard-account.md)Rolle Konto erstellen, während [!UICONTROL TV Tube] ein Konto mit der Publisher-Rolle erstellt.

Nach der Einrichtung ihrer Konten müssen sowohl [!UICONTROL Luma] als auch [!UICONTROL TV Tube] eine [Datenverbindung und Quell-Zielgruppen) &#x200B;](../setup/onboard-audiences.md). Nur [!UICONTROL TV Tube] aktiviert Zielgruppen für Marketing-Kampagnen. Daher müssen sie [ein Ziel konfigurieren](../setup/manage-destinations.md).

Sobald die Konten beider Mitarbeiter eingerichtet sind, können sie innerhalb der Plattform [eine Verbindung &#x200B;](../connect/establishing-connections.md). [!UICONTROL Luma] verwendet die [Discover Collaborators](../connect/discover-collaborators.md)-Funktion, um [!UICONTROL TV Tube] zu finden und eine Verbindungsanfrage zu initiieren. Nachdem [!UICONTROL TV Tube] die Verbindungsanfrage akzeptiert hat, konfiguriert [!UICONTROL Luma] die Verbindungseinstellungen, um zu definieren, wie sie zusammenarbeiten werden. [!UICONTROL TV Tube] akzeptiert die Verbindungsanfrage, um eine sichere Verbindung zwischen den beiden Marken herzustellen.

Nachdem die Verbindung hergestellt wurde, [!UICONTROL Luma] [erstellt ein Projekt](../collaborate/manage-projects.md) um ihre Zusammenarbeit mit [!UICONTROL TV Tube] zu starten. Während der Projekteinrichtung wählen sie die Anwendungsfälle für die Zusammenarbeit aus, die ihren Zielen am besten entsprechen: [Entdecken](../collaborate/discover.md), [Aktivieren](../collaborate/activate.md) und [Messen](../collaborate/measure.md).

[!UICONTROL Luma] nutzt das [Entdecken](../collaborate/discover.md)-Anwendungsbeispiel, um Einblicke in die Zielgruppendaten [!UICONTROL TV Tube] zu erhalten. Nachdem [!UICONTROL Luma] die Zielgruppensegmente identifiziert hat, [&#x200B; sie diese Zielgruppen &#x200B;](../collaborate/activate.md).

Nach der Aktivierung der Zielgruppen führt [!UICONTROL TV Tube] zielgerichtete Marketing-Kampagnen durch und lädt Daten in [Measure](../collaborate/measure.md) hoch, um die Effektivität der Kampagne zu bewerten.

## Marken-zu-Marken-Workflow {#brand-to-brand-workflow}

[!UICONTROL Fit Apparel], eine Sportbekleidungsmarke, möchte mit [!UICONTROL Luma], einer anderen Sportbekleidungsmarke, zusammenarbeiten, um Zielgruppendaten und Einblicke für verbesserte Marketing-Maßnahmen zu teilen.

Nach der Einrichtung ihrer Konten müssen sowohl [!UICONTROL Fit Apparel] als [!UICONTROL Luma] eine [&#x200B; und eine Quellzielgruppe &#x200B;](../setup/onboard-audiences.md). Sowohl [!UICONTROL Fit Apparel] als [!UICONTROL Luma] werden Zielgruppen für Marketing-Kampagnen aktivieren, sodass beide [Ziel konfigurieren](../setup/manage-destinations.md).

Nachdem sie ihre Zielgruppen abgerufen haben, [!UICONTROL Fit Apparel] und [!UICONTROL Luma] [eine Verbindung &#x200B;](../connect/establishing-connections.md) der Plattform, um Zielgruppendaten sicher freizugeben. Dazu müssen sie die Funktion „Einladung zur privaten [&quot; &#x200B;](../connect/establishing-connections.md#private-connection-invite). [!UICONTROL Luma] gibt ihren Verbindungs-Code an [!UICONTROL Fit Apparel] weiter, der ihn dann verwendet, um eine Verbindungsanfrage zu initiieren. Nachdem [!UICONTROL Luma] die Verbindungsanfrage akzeptiert hat, konfiguriert [!UICONTROL Fit Apparel] die Verbindungseinstellungen, um zu definieren, wie sie zusammenarbeiten werden. In der Konfiguration gibt [!UICONTROL Bekleidung anpassen] an, dass beide Mitarbeiter Zielgruppen für Marketing-Kampagnen aktivieren können. Um die Verbindung abzuschließen, [!UICONTROL Luma] akzeptiert die Anfrage, eine sichere Verbindung zwischen den beiden Marken herzustellen.

Nachdem die Verbindung hergestellt wurde, [!UICONTROL Fit Apparel] [erstellt ein Projekt](../collaborate/manage-projects.md) um ihre Zusammenarbeit mit [!UICONTROL Luma] zu starten. Während der Projekteinrichtung wählen sie die Anwendungsfälle für die Zusammenarbeit aus, die ihren Zielen am besten entsprechen: [Entdecken](../collaborate/discover.md), [Aktivieren](../collaborate/activate.md) und [Messen](../collaborate/measure.md).

[!UICONTROL Fit Apparel] und [!UICONTROL Luma] können beide den Anwendungsfall [Entdecken](../collaborate/discover.md) verwenden, um Einblicke in die Zielgruppendaten des anderen zu erhalten. Nachdem sie wertvolle Zielgruppensegmente identifiziert haben, [&#x200B; sie ihre &#x200B;](../collaborate/activate.md) Zielgruppen für Marketing-Kampagnen (aktivieren).

Schließlich laden beide Marken nach der Durchführung ihrer Kampagnen Daten in [Measure](../collaborate/measure.md) hoch und bewerten die Effektivität ihrer Zusammenarbeit.

## Workflow zwischen Werbetreibenden und Werbeplattformen {#advertiser-to-advertising-platform-workflow}

[!UICONTROL Luma], ein Sporteinzelhandelsunternehmen, möchte eine Verbindung zu [!DNL Amazon Marketing Cloud] ([!DNL AMC]) herstellen, um seine Marketing-Funktionen zu verbessern, indem es die Identitätsauflösungs- und Targeting-Tools von [!DNL AMC] nutzt. Luma hat bereits ein aktives [!DNL Amazon Advertising]-Konto und ist für die Verwendung von [!DNL AMC] zugelassen.

Zunächst muss [!UICONTROL Luma] ein [-Konto &#x200B;](../setup/onboard-account.md) der Rolle des Advertisers erstellen. Nach der Einrichtung des Kontos [!UICONTROL Luma] muss [eine Datenverbindung und Quellzielgruppen erstellen](../setup/onboard-audiences.md). Da [!UICONTROL Luma] Zielgruppen für Marketing-Kampagnen aktiviert, müssen sie [ein Ziel konfigurieren](../setup/manage-destinations.md).

Sobald [!UICONTROL Luma] ihr Konto eingerichtet hat, können sie mit [!DNL AMC] innerhalb der Plattform [eine Verbindung &#x200B;](../connect/establishing-connections.md). [!UICONTROL Luma] verwendet die [Discover Collaborators](../connect/discover-collaborators.md)-Funktion, um [!UICONTROL Amazon Marketing Cloud] zu finden und [eine Verbindungsanfrage zu starten](../connect/advertising-platforms/amc.md). Nach der Authentifizierung und Autorisierung der Verbindung über die [!DNL Amazon] Anmeldeseite wird die Verbindung mit [!DNL AMC] hergestellt.

Nachdem die Verbindung hergestellt wurde, [!UICONTROL Luma] [erstellt ein Projekt](../collaborate/manage-projects.md) um die Zusammenarbeit mit [!DNL AMC] zu starten. Die Verbindungseinstellungen, einschließlich der Anwendungsfälle, sind je nach Werbeplattform vorkonfiguriert. [!DNL AMC] ist der verfügbare Anwendungsfall &quot;[&quot; &#x200B;](../collaborate/advertising-platforms/amc.md#discover).

[!UICONTROL Luma] nutzt das [Entdecken](../collaborate/advertising-platforms/amc.md#discover)-Anwendungsbeispiel, um Einblicke und Zielgruppendaten aus [!DNL AMC] zu gewinnen. Mithilfe dieser Erkenntnisse kann [!UICONTROL Luma] seine Marketing-Strategien optimieren und die Effektivität der Kampagne verbessern.

## Workflow zwischen Advertiser und Datenpartner {#advertiser-to-data-partner-workflow}

[!UICONTROL Luma], ein Sporteinzelhandelsunternehmen, möchte mit [!UICONTROL DataM8], einem Drittanbieter von Daten, zusammenarbeiten, um Kundenprofile anzureichern und das Zielgruppen-Targeting zu verbessern.

Zunächst muss [!UICONTROL Luma] mit der Advertiser[&#128279;](../setup/onboard-account.md)Rolle Konto erstellen, während [!UICONTROL DataM8] ein Konto mit der Datenpartnerrolle erstellt.

Nach der Einrichtung der Konten müssen sowohl [!UICONTROL Luma] als [!UICONTROL DataM8] eine [&#x200B; und Quell-Zielgruppen &#x200B;](../setup/onboard-audiences.md). Beide Mitarbeiter können Zielgruppen für Marketing-Kampagnen aktivieren, sodass sie jeweils ein [&#x200B; konfigurieren &#x200B;](../setup/manage-destinations.md).

Sobald die Konten beider Mitarbeiter eingerichtet sind, können sie innerhalb der Plattform [eine Verbindung &#x200B;](../connect/establishing-connections.md). [!UICONTROL Luma] verwendet die [Discover Collaborators](../collaborate/discover.md)-Funktion, um [!UICONTROL DataM8] zu finden und eine Verbindungsanfrage zu initiieren. Nachdem [!UICONTROL DataM8] die Verbindungsanfrage akzeptiert hat, konfiguriert [!UICONTROL Luma] die Verbindungseinstellungen, um zu definieren, wie sie zusammenarbeiten werden. [!UICONTROL DataM8] akzeptiert die Verbindungsanfrage, um eine sichere Verbindung zwischen den beiden Partnern herzustellen.

Nachdem die Verbindung hergestellt wurde, [!UICONTROL Luma] [erstellt ein Projekt](../collaborate/manage-projects.md) um die Zusammenarbeit mit [!UICONTROL DataM8] zu starten. Während der Projekteinrichtung wählen sie die Anwendungsfälle für die Zusammenarbeit aus, die ihren Zielen am besten entsprechen: [Entdecken](../collaborate/discover.md), [Aktivieren](../collaborate/activate.md) und [Messen](../collaborate/measure.md).

[!UICONTROL Luma] nutzt das [Discover](../collaborate/discover.md)-Anwendungsbeispiel, um Einblicke in die Zielgruppendaten [!UICONTROL DataM8] zu erhalten. Nachdem [!UICONTROL Luma] die Zielgruppensegmente identifiziert hat, [&#x200B; sie diese &#x200B;](../collaborate/activate.md).

[!UICONTROL DataM8] kann auch [aktivieren](../collaborate/activate.md) seine Zielgruppen für [!UICONTROL Luma]. [!UICONTROL Luma] nutzt diese Funktionen, um Attribute von Drittanbietern an seine Kundenprofile anzuhängen und die Komposition von Audiences zu analysieren. Wenn angereicherte Daten direkt in der CDP verfügbar sind, [!UICONTROL Luma] präzisere Zielgruppen erstellen und diese für Paid-Media-Ziele aktivieren, ohne Daten aus der verwalteten Umgebung zu verschieben.

## Workflow „Agentur-zu-Publisher“ {#agency-to-publisher-workflow}

[!UICONTROL Agency99], eine Medienagentur, möchte mit [!UICONTROL TV Tube], einem digitalen Streaming-Anbieter, zusammenarbeiten, um bestimmte Zielgruppen durch zielgerichtete Marketing-Kampagnen zu erreichen.

Zunächst muss [!UICONTROL Agency99] mit der Agenturrolle [Konto erstellen](../setup/onboard-account.md) während [!UICONTROL TV Tube] ein Konto mit der Publisher-Rolle erstellt.

Nach der Einrichtung ihrer Konten müssen sowohl [!UICONTROL Agency99] als [!UICONTROL TV Tube] eine [Datenverbindung und Quell-Zielgruppen) &#x200B;](../setup/onboard-audiences.md). [!UICONTROL Agency99] wird in seinem Arbeitsbereich Client-Unterkonten und Client-Quelldaten einrichten. Nur [!UICONTROL TV Tube] aktiviert Zielgruppen für Marketing-Kampagnen. Daher müssen sie [ein Ziel konfigurieren](../setup/manage-destinations.md).

Sobald die Konten beider Mitarbeiter eingerichtet sind, können sie innerhalb der Plattform [eine Verbindung &#x200B;](../connect/establishing-connections.md). [!UICONTROL Agency99] verwendet die [Discover Collaborators](../collaborate/discover.md)-Funktion, um [!UICONTROL TV Tube] zu finden und eine Verbindungsanfrage zu initiieren. [!UICONTROL Agency99] wird dies für einen oder mehrere Kunden tun, die mit (TV Tube[!UICONTROL &#x200B; zusammenarbeiten &#x200B;]. Nachdem [!UICONTROL TV Tube] die Verbindungsanfrage(n) akzeptiert hat, konfiguriert [!UICONTROL Agency99] die Verbindungseinstellungen, um festzulegen, wie jede Zusammenarbeit funktioniert. [!UICONTROL TV Tube] akzeptiert die Verbindungsanfrage(n), um eine sichere Verbindung zwischen den beiden Marken herzustellen.

Nachdem die Verbindung hergestellt wurde[!UICONTROL &#x200B; erstellt &#x200B;][Agency99) ein Projekt](../collaborate/manage-projects.md) um die Zusammenarbeit mit [!UICONTROL TV Tube] in jedem Client-Unterkonto zu starten. Während der Projekteinrichtung wählen sie die Anwendungsfälle für die Zusammenarbeit aus, die ihren Zielen am besten entsprechen: [Entdecken](../collaborate/discover.md), [Aktivieren](../collaborate/activate.md) und [Messen](../collaborate/measure.md).

[!UICONTROL Agency99] nutzt das [Discover](../collaborate/discover.md)-Anwendungsbeispiel, um Einblicke in die Zielgruppendaten [!UICONTROL TV Tube] zu erhalten. Nachdem [!UICONTROL Agency99] die Zielgruppensegmente identifiziert hat, [&#x200B; sie diese Zielgruppen &#x200B;](../collaborate/activate.md).

Nach der Aktivierung der Zielgruppen führt [!UICONTROL TV Tube] zielgerichtete Marketing-Kampagnen durch und lädt Daten hoch, um [&#x200B; Ergebnisse &#x200B;](../collaborate/measure.md) messen, um die Effektivität ihrer Kampagne zu bewerten.

## Workflow zwischen Advertiser und Agentur {#advertiser-to-agency-platform-workflow}

[!UICONTROL Luma], ein athletisches Einzelhandelsunternehmen, möchte mit [!UICONTROL Holdco], einer Agenturplattform, zusammenarbeiten, um Daten auszutauschen und Paid-Media-Einblicke zu erhalten.

Zunächst muss [!UICONTROL Luma] ein [Konto erstellen](../setup/onboard-account.md) mit der Rolle des Advertisers erstellen, während [!UICONTROL Holdco] ein Konto mit der Rolle der Agentur erstellt. 

Nach der Einrichtung ihrer Konten müssen sowohl [!UICONTROL Luma] als [!UICONTROL Holdco] [eine Datenverbindung und Quellzielgruppen erstellen](../setup/onboard-audiences.md). Beide Mitarbeiter können Zielgruppen für Marketing-Kampagnen aktivieren, sodass sie jeweils ein [&#x200B; konfigurieren &#x200B;](../setup/manage-destinations.md). 

Sobald die Konten beider Mitarbeiter eingerichtet sind, können sie innerhalb der Plattform [eine Verbindung &#x200B;](../connect/establishing-connections.md). [!UICONTROL Luma] verwendet die Funktion [Discover Collaborators](../collaborate/discover.md), um [!UICONTROL Holdco] zu finden und eine Verbindungsanfrage zu initiieren. Nachdem [!UICONTROL Holdco] die Verbindungsanfrage akzeptiert hat, konfiguriert [!UICONTROL Luma] die Verbindungseinstellungen, um zu definieren, wie sie zusammenarbeiten werden.

[!UICONTROL Holdco] akzeptiert die Verbindungsanfrage, um eine sichere Verbindung zwischen den beiden Partnern herzustellen.

Nachdem die Verbindung hergestellt wurde, [!UICONTROL Luma] [erstellt ein Projekt](../collaborate/manage-projects.md) um ihre Zusammenarbeit mit [!UICONTROL Holdco] zu starten. Während der Projekteinrichtung wählen sie die Anwendungsfälle für die Zusammenarbeit aus, die ihren Zielen am besten entsprechen: [Entdecken](../collaborate/discover.md), [Aktivieren](../collaborate/activate.md) und [Messen](../collaborate/measure.md).

[!UICONTROL Luma] nutzt das [Entdecken](../collaborate/discover.md)-Anwendungsbeispiel, um Einblicke in die Zielgruppendaten [!UICONTROL Holdco] zu erhalten. Nachdem [!UICONTROL Luma] die Zielgruppensegmente identifiziert hat, [&#x200B; sie diese &#x200B;](../collaborate/activate.md).

[!UICONTROL Holdco] kann auch [aktivieren](../collaborate/activate.md) seine Zielgruppen auf [!UICONTROL Luma]. [!UICONTROL Luma] nutzt diese Funktionen, um Paid-Media-Einblicke aus von Agenturen durchgeführten Kampagnen für Einblicke, CDP-Profilanhänge und die Orchestrierung eigener Medien zu erhalten.
