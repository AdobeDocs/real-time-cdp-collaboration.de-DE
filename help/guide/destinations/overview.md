---
title: Ziele - Übersicht
description: Erfahren Sie mehr über Ziele in Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 5cbbf5c4-4caa-40da-97be-690d95c1201c
TQID: https://experienceleague.adobe.com/1VvnSt3Z65dfQBfXnjJJi3H0Oj9BxFStexq3icVKxkY
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2: id: b5520579-b31f-4df7-9281-f0d9f91e2edcid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 7ab1bc21a4d644e2e6a481d8de594d6a509a92a5
workflow-type: tm+mt
source-wordcount: 273
ht-degree: 6%

---

# Ziele – Übersicht

{{limited-availability-release-note}}

>[!NOTE]
>
>Auf dieser Seite werden Ziele behandelt, für die Zielgruppen aktiviert ****, z. B. Cloud-Speicherplattformen. Informationen zum Aktivieren von Zielgruppen **für einen Mitwirkenden** in einem freigegebenen Projekt finden Sie im [Aktivieren von Zielgruppen](/help/guide/collaborate/activate.md).

Ziele sind Integrationen, die zum Senden zielgerichteter Zielgruppen an externe Plattformen verwendet werden. Mit diesen Integrationen können Sie Zielgruppen über verschiedene Marketing-Kanäle und Plattformen hinweg aktivieren, um sie in Kampagnen und bei der Kundeninteraktion zu verwenden.

Mitwirkende können Ziele konfigurieren, um Zielgruppen an externe Plattformen wie Adobe Experience Platform oder eine Cloud-Speicherplattform zur Verwendung in Kampagnen zu senden. Mitwirkende können dann [Zielgruppen innerhalb eines Projekts aktivieren](../collaborate/activate.md) die an das konfigurierte Ziel ihrer Verbindung gesendet werden. Die Aktivierung kann je nach den in der Verbindung konfigurierten Zielgruppen-Aktivierungseinstellungen [ Mitarbeiter ](/help/guide/connect/establishing-connections.md#configure-connection-settings).

>[!IMPORTANT]
>
>Wenn Mitwirkende Zielgruppen in einem Projekt aktivieren, werden sie derzeit automatisch an das konfigurierte Ziel ihrer Verbindung gesendet. Sie **müssen** ein Ziel konfigurieren, bevor Ihr Mitarbeiter Zielgruppen innerhalb eines Projekts aktivieren kann.

## Verfügbare Ziele {#available-destinations}

Die folgenden Ziele sind für die Konfiguration in Collaboration verfügbar. Um das Konfigurationshandbuch für dieses Ziel anzuzeigen, wählen Sie den Zielnamen in der folgenden Tabelle aus.

| Ziel | Verfügbarkeit |
| --- | --- |
| [Adobe Experience Platform](./experience-platform.md) | Verfügbar |
| [[!DNL Amazon S3]](./manage-destinations.md) | Verfügbar |
| [[!DNL Snowflake]](./manage-destinations.md) | Verfügbar |
| [[!DNL Google Cloud Storage]](./manage-destinations.md) | Verfügbar |
| [[!DNL Azure Blob Storage]](./manage-destinations.md) | Verfügbar |
| [[!DNL SFTP]](./manage-destinations.md) | Verfügbar |
| [[!DNL Data Landing Zone]](./manage-destinations.md) | Verfügbar |

>[!NOTE]
>
>**[!DNL Google Cloud Storage]** dieser Tabelle bezieht sich auf **Ziele** (bei denen Collaboration Zielgruppen während der Aktivierung sendet). Informationen **„Beschaffung von Zielgruppen** einem GCS-Bucket im **[!UICONTROL Setup]**-Arbeitsbereich finden Sie unter [Konfigurieren von GCS für die Zielgruppen-Beschaffung](../setup/configure-gcs-audience-sourcing.md).

## Nächste Schritte

Informationen zum Konfigurieren eines Ziels finden Sie im [Konfigurieren und Verwalten eines Ziels](./manage-destinations.md). Nachdem Sie Ihr Ziel konfiguriert haben, können Sie mit der [Aktivierung zielgerichteter Zielgruppen](../collaborate/activate.md) in Ihren Projekten beginnen.
