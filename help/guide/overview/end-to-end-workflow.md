---
title: End-to-End-Workflow
description: Machen Sie sich mit dem End-to-End-Workflow der Verwendung von Real-Time CDP Collaboration auf der Grundlage Ihres Kooperationsmusters vertraut.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
source-git-commit: 8745d6d8da389b552af3da6612bf693230dfb538
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# End-to-End-Workflow

{{limited-availability-release-note}}

In Adobe Real-Time CDP Collaboration variiert der End-to-End-Workflow je nach ausgewähltem Zusammenarbeitsmuster. Der Workflow beschreibt die Schritte, die bei der Einrichtung und Ausführung eines Collaboration-Projekts erforderlich sind, von der Erstellung von Konten und der Beschaffung von Zielgruppen bis hin zur Herstellung von Verbindungen und zur Erstellung von Projekten. Das Verständnis dieses Workflows ist von entscheidender Bedeutung, um die Funktionen der Plattform effektiv nutzen zu können, um Ihre Marketing-Ziele zu erreichen.

## Erste Schritte

Bevor Sie beginnen, stellen Sie sicher, dass Sie über ein solides Verständnis dieser Schlüsselkonzepte verfügen:

- **Collaboration-Muster**: Diese Muster definieren, wie Kollaborateure zusammenarbeiten. Es gibt zwei verschiedene Muster[ „Advertiser-](./collaboration-patterns.md#advertiser-to-publisher)&quot; und [Marke-zu-Marke](./collaboration-patterns.md#brand-to-brand).
- **Kontorollen**: Kontorollen bestimmen Ihre Funktionen innerhalb der Plattform. Sie sollten mit den Zielen, der Marke und den Zielen Ihres Unternehmens übereinstimmen. Es gibt zwei Kontorollen: [Advertiser](./roles.md#advertiser) und [Publisher](./roles.md#publisher).
- **Anwendungsfälle**: Anwendungsfälle definieren, wie Sie Collaboration zum Erreichen Ihrer Marketing-Ziele nutzen können. Es gibt drei Anwendungsfälle für die Zusammenarbeit: [Entdecken](./use-cases.md#discover), [Aktivieren](./use-cases.md#activate) und [Messen](./use-cases.md#measure).

In diesem Handbuch werden drei Pseudo-Kollaborateure verwendet, um den End-to-End-Workflow zu veranschaulichen:

- **[!UICONTROL Luma]**: Eine Sportbekleidungsmarke. Sie sind ein Advertiser, der durch zielgerichtete Marketing-Kampagnen bestimmte Zielgruppen erreichen möchte.
- **[!UICONTROL TV Tube]**: Ein digitaler Streaming-Anbieter. Sie sind ein Publisher, der Zielgruppendaten für die Verwendung durch Advertiser bereitstellt.
- **[!UICONTROL Fit Apparel]**: Eine weitere Sportbekleidungsmarke. Sie sind ein zweiter Werbetreibender, der zusammenarbeiten möchte, um Zielgruppendaten und Einblicke für verbesserte Marketing-Maßnahmen zu teilen.

## Workflow von Advertiser zu Publisher {#advertiser-to-publisher-workflow}

[!UICONTROL Luma], ein Sporteinzelhandelsunternehmen, möchte eine Verbindung mit [!UICONTROL TV Tube], einem digitalen Streaming-Anbieter, herstellen, um bestimmte Zielgruppen durch zielgerichtete Marketing-Kampagnen zu erreichen.

Zunächst muss [!UICONTROL Luma] mit der Advertiser[Rolle ](../setup/onboard-account.md)Konto erstellen, während [!UICONTROL TV Tube] ein Konto mit der Publisher-Rolle erstellt.

Nach der Einrichtung ihrer Konten müssen sowohl [!UICONTROL Luma] als auch [!UICONTROL TV Tube] eine [Datenverbindung und Quell-Zielgruppen) ](../setup/onboard-audiences.md). Nur [!UICONTROL TV Tube] aktiviert Zielgruppen für Marketing-Kampagnen. Daher müssen sie [ein Ziel konfigurieren](../setup/manage-destinations.md).

Sobald die Konten beider Mitarbeiter eingerichtet sind, können sie innerhalb der Plattform [eine Verbindung ](../connect/establishing-connections.md). [!UICONTROL Luma] verwendet die [Discover Publishers](../connect/discover-publishers.md)-Funktion, um [!UICONTROL TV Tube] zu finden und eine Verbindungsanfrage zu initiieren. Nachdem [!UICONTROL TV Tube] die Verbindungsanfrage akzeptiert hat, konfiguriert [!UICONTROL Luma] die Verbindungseinstellungen, um zu definieren, wie die Zusammenarbeit funktioniert. [!UICONTROL TV Tube] akzeptiert die Verbindungsanfrage, um eine sichere Verbindung zwischen den beiden Marken herzustellen.

Nachdem die Verbindung hergestellt wurde, [!UICONTROL Luma] [erstellt ein Projekt](../collaborate/manage-projects.md) um ihre Zusammenarbeit mit [!UICONTROL TV Tube] zu starten. Während der Projekteinrichtung wählen sie die Anwendungsfälle für die Zusammenarbeit aus, die ihren Zielen am besten entsprechen: [Entdecken](../collaborate/discover.md), [Aktivieren](../collaborate/activate.md) und [Messen](../collaborate/measure.md).

[!UICONTROL Luma] nutzt das [Entdecken](../collaborate/discover.md)-Anwendungsbeispiel, um Einblicke in die Zielgruppendaten [!UICONTROL TV Tube] zu erhalten. Nachdem [!UICONTROL Luma] die Zielgruppensegmente identifiziert hat, [ sie diese Zielgruppen ](../collaborate/activate.md).

Nach der Aktivierung der Zielgruppen führt [!UICONTROL TV Tube] zielgerichtete Marketing-Kampagnen durch und lädt Daten in [Measure](../collaborate/measure.md) hoch, um die Effektivität der Kampagne zu bewerten.

## Marken-zu-Marken-Workflow {#brand-to-brand-workflow}

[!UICONTROL Fit Apparel], eine Sportbekleidungsmarke, möchte mit [!UICONTROL Luma], einer anderen Sportbekleidungsmarke, zusammenarbeiten, um Zielgruppendaten und Einblicke für verbesserte Marketing-Maßnahmen zu teilen.

Nach der Einrichtung ihrer Konten müssen sowohl [!UICONTROL Fit Apparel] als [!UICONTROL Luma] eine [ und eine Quellzielgruppe ](../setup/onboard-audiences.md). Sowohl [!UICONTROL Fit Apparel] als [!UICONTROL Luma] werden Zielgruppen für Marketing-Kampagnen aktivieren, sodass beide [Ziel konfigurieren](../setup/manage-destinations.md).

Nachdem sie ihre Zielgruppen abgerufen haben, [!UICONTROL Fit Apparel] und [!UICONTROL Luma] [eine Verbindung ](../connect/establishing-connections.md) der Plattform, um Zielgruppendaten sicher freizugeben. Dazu müssen sie die Funktion „Einladung zur privaten [&quot; ](../connect/establishing-connections.md#private-connection-invite). [!UICONTROL Luma] gibt ihren Verbindungs-Code an [!UICONTROL Fit Apparel] weiter, der ihn dann verwendet, um eine Verbindungsanfrage zu initiieren. Nachdem [!UICONTROL Luma] die Verbindungsanfrage akzeptiert hat, konfiguriert [!UICONTROL Fit Apparel] die Verbindungseinstellungen, um zu definieren, wie sie zusammenarbeiten werden. In der Konfiguration gibt [!UICONTROL Bekleidung anpassen] an, dass beide Mitarbeiter Zielgruppen für Marketing-Kampagnen aktivieren können. Um die Verbindung abzuschließen, [!UICONTROL Luma] akzeptiert die Anfrage, eine sichere Verbindung zwischen den beiden Marken herzustellen.

Nachdem die Verbindung hergestellt wurde, [!UICONTROL Fit Apparel] [erstellt ein Projekt](../collaborate/manage-projects.md) um ihre Zusammenarbeit mit [!UICONTROL Luma] zu starten. Während der Projekteinrichtung wählen sie die Anwendungsfälle für die Zusammenarbeit aus, die ihren Zielen am besten entsprechen: [Entdecken](../collaborate/discover.md), [Aktivieren](../collaborate/activate.md) und [Messen](../collaborate/measure.md).

[!UICONTROL Fit Apparel] und [!UICONTROL Luma] können beide den Anwendungsfall [Entdecken](../collaborate/discover.md) verwenden, um Einblicke in die Zielgruppendaten des anderen zu erhalten. Nachdem sie wertvolle Zielgruppensegmente identifiziert haben, [ sie ihre ](../collaborate/activate.md) Zielgruppen für Marketing-Kampagnen (aktivieren).

Schließlich laden beide Marken nach der Durchführung ihrer Kampagnen Daten in [Measure](../collaborate/measure.md) hoch und bewerten die Effektivität ihrer Zusammenarbeit.
