---
title: Konfigurieren und Verwalten von Zielen
description: Erfahren Sie, wie Sie Ziele in Real-Time CDP Collaboration konfigurieren und verwalten.
audience: admin, publisher
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b4b26761-46ac-420f-b9f7-6e829d67aec9
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 1%

---

# Konfigurieren und Verwalten von Zielen

{{limited-availability-release-note}}

Ziele sind Integrationen, die zum Senden zielgerichteter Zielgruppen an externe Plattformen verwendet werden. Mit diesen Integrationen können Sie Zielgruppen über verschiedene Marketing-Kanäle und Plattformen hinweg aktivieren, um sie in Kampagnen und bei der Kundeninteraktion zu verwenden.

Derzeit sind Ziele nur für Publisher in Real-Time CDP Collaboration verfügbar. Herausgeber können Ziele konfigurieren, um Zielgruppen auf externen Plattformen wie Adobe Experience Platform für die Verwendung in Kampagnen zu aktivieren. Werbetreibende können dann [Zielgruppen innerhalb eines Projekts senden](../collaborate/activate.md) die an das konfigurierte Ziel des Herausgebers gesendet werden.

![Auf der Registerkarte „Meine Ziele“ im Setup-Arbeitsbereich werden aktive Adobe Experience Platform-Ziele angezeigt.](/help/assets/setup/manage-destinations/my-destinations-overview.png)

Weitere Informationen zu Zielen finden Sie im Handbuch [Ziele - Übersicht](../destinations/overview.md).

## Konfigurieren von Zielen {#configure-destinations}

Ziele werden im Abschnitt **[!UICONTROL Setup]** von Collaboration konfiguriert. Um ein Ziel zu konfigurieren, navigieren Sie zu **[!UICONTROL Setup]** und wählen Sie dann die Registerkarte **[!UICONTROL Meine Ziele]** aus. Hier können Sie alle verfügbaren Ziele anzeigen.

>[!IMPORTANT]
>
>Um Ziele zu konfigurieren und zu verwalten, muss Ihren Benutzenden eine Rolle mit der Berechtigung **Verwalten von Zielgruppendaten** zugewiesen sein. Weitere Informationen zur Verwaltung von Rollen finden Sie im [Rollen verwalten](../permissions/manage-roles.md).

![Auf der Registerkarte „Meine Ziele“ im Setup-Arbeitsbereich werden die verfügbaren Ziele angezeigt.](/help/assets/setup/manage-destinations/my-destinations.png)

Der Einrichtungsprozess für Ziele hängt vom Ziel ab, das Sie konfigurieren. Siehe den Katalog [Verfügbare Ziele](../destinations/overview.md#available-destinations), um die verfügbaren Ziele und ihre Konfigurationshandbücher anzuzeigen.

>[!NOTE]
>
>Derzeit ist in Real-Time CDP Collaboration nur Adobe Experience Platform als Self-Service-Ziel verfügbar. Wenn Sie ein anderes Ziel konfigurieren möchten, wenden Sie sich an Ihren Adobe-Support-Mitarbeiter.

## Löschen von Zielen {#delete-destinations}

Wenn Sie ein Ziel löschen, wird es aus Ihrer Organisation entfernt, alle zuvor gesendeten Zielgruppen werden aus dem Ziel entfernt und es wird verhindert, dass zukünftige Zielgruppen an dieses Ziel gesendet werden.

Um ein Ziel zu löschen, navigieren Sie zur Registerkarte **[!UICONTROL Meine Ziele]** im Abschnitt **[!UICONTROL Setup]**. Wählen Sie die **[!UICONTROL Löschen]** für das Ziel aus, das Sie entfernen möchten.

![Der Arbeitsbereich „Meine Ziele“ mit hervorgehobener Option „Löschen“ für das Adobe Experience Platform-Ziel.](/help/assets/setup/manage-destinations/delete-destination.png)

Es wird ein Bestätigungsdialogfeld angezeigt, in dem Sie bestätigen können, dass Sie das Ziel löschen möchten. Wählen Sie **[!UICONTROL Löschen]** aus, um das Ziel zu entfernen.

![Das Dialogfeld „Ziel löschen“ mit hervorgehobener Option „Löschen“.](/help/assets/setup/manage-destinations/delete-destination-confirmation.png)

## Nächste Schritte

Nachdem Sie Ihr Ziel konfiguriert haben, können Sie mit Ihren Advertisern zusammenarbeiten, um [ Zielgruppen in ](../collaborate/activate.md) Projekten zu aktivieren.
