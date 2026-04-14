---
title: Ziele - Übersicht
description: Erfahren Sie mehr über Ziele in Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 5cbbf5c4-4caa-40da-97be-690d95c1201c
source-git-commit: 87e7feb1360d905d46032b49217f3cfee4cc6d6b
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 3%

---

# Ziele – Übersicht

{{limited-availability-release-note}}

Ziele sind Integrationen, die zum Senden zielgerichteter Zielgruppen an externe Plattformen verwendet werden. Mit diesen Integrationen können Sie Zielgruppen über verschiedene Marketing-Kanäle und Plattformen hinweg aktivieren, um sie in Kampagnen und bei der Kundeninteraktion zu verwenden.

Mitwirkende können Ziele konfigurieren, um Zielgruppen zur Verwendung in Kampagnen an externe Plattformen wie Adobe Experience Platform zu senden. Mitwirkende können dann [Zielgruppen innerhalb eines Projekts aktivieren](../collaborate/activate.md) die an das konfigurierte Ziel ihrer Verbindung gesendet werden. Die Aktivierung kann je nach den in der Verbindung konfigurierten Zielgruppen-Aktivierungseinstellungen [&#x200B; Mitarbeiter &#x200B;](/help/guide/connect/establishing-connections.md#configure-connection-settings).

>[!IMPORTANT]
>
>Wenn Mitwirkende Zielgruppen in einem Projekt aktivieren, werden sie derzeit automatisch an das konfigurierte Ziel ihrer Verbindung gesendet. Sie **müssen** ein Ziel konfigurieren, bevor Ihr Mitarbeiter Zielgruppen innerhalb eines Projekts aktivieren kann.

## Konfigurieren von Zielen {#configure-destinations}

Um ein Ziel zu konfigurieren, navigieren Sie zu **[!UICONTROL Setup]** und wählen Sie dann die Registerkarte **[!UICONTROL Meine Ziele]** aus. Hier können Sie alle verfügbaren Ziele anzeigen.

>[!NOTE]
>
> Derzeit ist in Collaboration nur Adobe Experience Platform als Self-Service-Ziel verfügbar. Wenn Sie an der Konfiguration eines Ziels wie Amazon S3 oder Snowflake interessiert sind, wenden Sie sich bitte an Ihren Adobe-Support-Mitarbeiter.

![Auf der Registerkarte „Meine Ziele“ im Setup-Arbeitsbereich werden die verfügbaren Ziele angezeigt.](/help/assets/destinations/overview/my-destinations-overview.png)

Um mit der Konfiguration eines Ziels zu beginnen **[!UICONTROL wählen Sie die Option]** Einrichten“ innerhalb des Ziels Ihrer Wahl aus. Informationen zur Konfiguration bestimmter Ziele finden Sie in den Handbüchern in der Tabelle [Verfügbare Ziele](#available-destinations).

![Der Arbeitsbereich „Meine Ziele“ mit der hervorgehobenen Option „Einrichten“ für das Adobe Experience Platform-Ziel.](/help/assets/destinations/overview/my-destinations-set-up.png)

### Verfügbare Ziele {#available-destinations}

Die folgenden Ziele sind für die Konfiguration in Collaboration verfügbar. Um das Konfigurationshandbuch für dieses Ziel anzuzeigen, wählen Sie den Zielnamen in der folgenden Tabelle aus. Wenn Sie an der Konfiguration eines Ziels interessiert sind, das derzeit nicht verfügbar ist, wenden Sie sich an den Adobe-Support.

| Ziel | Verfügbarkeit |
| --- | --- |
| [Adobe Experience Platform](./experience-platform.md) | Verfügbar |
| [!DNL Amazon S3] | Bald verfügbar. |
| [!DNL Snowflake] | Bald verfügbar. |
| [!DNL Google Cloud Storage] | Bald verfügbar. |
| [!DNL Azure Blob Storage] | Bald verfügbar. |

>[!NOTE]
>
>**[!DNL Google Cloud Storage]** dieser Tabelle bezieht sich auf **Ziele** (bei denen Collaboration Zielgruppen während der Aktivierung sendet). Informationen **„Beschaffung von Zielgruppen** einem GCS-Bucket im **[!UICONTROL Setup]**-Arbeitsbereich finden Sie unter [Konfigurieren von GCS für die Zielgruppen-Beschaffung](../setup/configure-gcs-audience-sourcing.md).

## Nächste Schritte

Nachdem Sie Ihr Ziel konfiguriert haben, können Sie mit der [Aktivierung zielgerichteter Zielgruppen](../collaborate/activate.md) in Ihren Projekten beginnen.
