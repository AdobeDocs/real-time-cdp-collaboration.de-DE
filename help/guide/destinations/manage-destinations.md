---
title: Konfigurieren und Verwalten von Cloud-Speicher-Zielen
description: Erfahren Sie, wie Sie ein Cloud-Speicher-Ziel in Real-Time CDP Collaboration konfigurieren, anzeigen und löschen.
audience: admin, publisher
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2: id: b5520579-b31f-4df7-9281-f0d9f91e2edcid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 60124235569ca9b17b3bb1cef502d57d39e82e1f
workflow-type: tm+mt
source-wordcount: 885
ht-degree: 1%

---

# Konfigurieren und Verwalten von Cloud-Speicher-Zielen

Verwenden Sie dieses Handbuch, um Cloud-Speicher-Ziele zu konfigurieren, anzuzeigen und aus dem Arbeitsbereich **[!UICONTROL Aktivierung]** zu löschen. Verwenden Sie die Registerkarte **[!UICONTROL Katalog]** zum Konfigurieren von Zielen, die Registerkarte **[!UICONTROL Ziele]** zum Verwalten dieser Ziele und die Registerkarte **[!UICONTROL Aktivierte Zielgruppen]** zum Überprüfen von für Ziele aktivierten Zielgruppen.

Nachdem Sie ein Ziel konfiguriert haben, wird es verfügbar, wenn Sie Zielgruppen aktivieren. Die vollständige Liste der unterstützten Ziele finden Sie in der Tabelle [Verfügbare Ziele](./overview.md#available-destinations).

>[!NOTE]
>
> In diesem Handbuch wird ein **[!DNL Amazon S3]**-Ziel als Beispiel verwendet. Der geführte Konfigurations-Workflow wird für alle unterstützten Cloud-Speicher-Zieltypen freigegeben, aber Authentifizierungsmethoden, erforderliche Felder und Connector-Funktionen können variieren. Bevor Sie ein Ziel konfigurieren, lesen Sie [Cloud-Speicher-Zielanforderungen](./cloud-storage-destination-requirements.md), die Sie mit der entsprechenden Adobe Experience Platform-Zieldokumentation verknüpfen.
>
> Adobe Experience Platform verfügt in Real-Time CDP Collaboration über einen separaten Konfigurations-Workflow. Informationen zur Konfiguration finden Sie unter [Konfigurieren von Adobe Experience Platform als Ziel](./experience-platform.md).

## Voraussetzungen {#prerequisites}

Bevor Sie ein Ziel konfigurieren, stellen Sie Folgendes sicher:

* Sie haben Zugriff auf den Arbeitsbereich **[!UICONTROL Aktivierung]**.
* Sie verfügen über die Verbindungsinformationen, die von Ihrem Cloud-Speicheranbieter benötigt werden.
* Wenn Sie ein Konto erstellen müssen, verfügen Sie über die erforderlichen Anmeldeinformationen oder Berechtigungen.
* Sie haben die [Anforderungen für Ihr Cloud-Speicherziel“ ](./cloud-storage-destination-requirements.md).

## Konfigurieren eines Ziels {#configure-destination}

Wenn Sie ein Ziel konfigurieren, verbinden Sie ein Cloud-Speicherkonto mit Real-Time CDP Collaboration und definieren, wie Zielgruppendaten in dieses exportiert werden.

Navigieren Sie **[!UICONTROL Aktivierung]** > **[!UICONTROL Katalog]**.

Auf **[!UICONTROL Registerkarte]** Katalog“ werden die verfügbaren Zielanbieter angezeigt. Jedes Ziel wird als Karte angezeigt. Je nach Ziel kann die zugehörige Karte konfigurierte Konten und Aktionen anzeigen, um zusätzliche Informationen anzuzeigen.

![Die Registerkarte Katalog mit Ziel-Provider-Karten.](/help/assets/destinations/manage-destinations/destination-provider-catalog.png)

Suchen Sie den Zielanbieter, den Sie konfigurieren möchten, und wählen Sie **[!UICONTROL Einrichten]**.

Das geführte Setup für die Zielkonfiguration wird geöffnet und führt Sie durch vier Schritte: **[!UICONTROL Authentifizieren]**, **[!UICONTROL Ziel erstellen]**, **[!UICONTROL Zuordnungsfelder]** und **[!UICONTROL Überprüfen]**.

### Authentifizieren {#authenticate}

Der **[!UICONTROL Authentifizieren]**-Schritt stellt eine Verbindung zwischen Real-Time CDP Collaboration und Ihrem Zielkonto her.

Wenn ein vorhandenes Konto verfügbar ist, wählen Sie es aus der Kontoauswahl aus. Um ein Konto zu erstellen, wählen Sie **[!UICONTROL Neues Konto]** aus.

Wählen Sie eine Authentifizierungsmethode aus und geben Sie die erforderlichen Kontoinformationen ein. Die verfügbaren Authentifizierungsmethoden und -felder hängen vom ausgewählten Zielanbieter ab. Informationen zu Connector-spezifischen Anforderungen finden Sie unter [Cloud-Speicherziel-Anforderungen](./cloud-storage-destination-requirements.md).

Wählen **[!UICONTROL Mit Amazon S3 verbinden]** aus. Für andere Zielanbieter zeigt die Schaltfläche den entsprechenden Anbieternamen an.

Nachdem das Konto erfolgreich validiert wurde, klicken Sie auf **[!UICONTROL Weiter]**.

![Der Schritt „Authentifizieren“ mit Kontoauswahl und Erstellung eines neuen Kontos.](/help/assets/destinations/manage-destinations/authenticate-destination-account.png)

### Ziel erstellen {#create-destination}

Der **[!UICONTROL Ziel erstellen]** definiert, wo und wie Zielgruppenexportdateien bereitgestellt werden.

Geben Sie einen Zielnamen ein und füllen Sie die erforderlichen Speicher- und Exporteinstellungen aus. Die verfügbaren Felder hängen vom ausgewählten Zielanbieter ab. Definitionen und Connector-spezifische Anforderungen finden Sie in der Zieldokumentation, die unter [Cloud-Speicherzielanforderungen“ ](./cloud-storage-destination-requirements.md) ist.

Nachdem Sie alle erforderlichen Felder ausgefüllt haben, klicken Sie auf **[!UICONTROL Weiter]**. Die geführte Einrichtung geht zum Schritt der Feldzuordnung über.

![Der Schritt „Ziel erstellen“ mit Feldern zur Zielkonfiguration.](/help/assets/destinations/manage-destinations/configure-new-destination.png)

### Zuordnen von Feldern {#map-fields}

Der Schritt **[!UICONTROL Felder zuordnen]** definiert, wie Schlüssel für die Zielgruppen-Übereinstimmung den vom Ziel erwarteten Identitätsfeldern zugeordnet werden.

Im Gegensatz zum standardmäßigen Real-Time CDP-Ziel-Workflow konfiguriert Real-Time CDP Collaboration diese Zuordnungen, während das Ziel erstellt wird. Schlüssel zur Zielgruppenübereinstimmung werden als Quellfelder angezeigt. Ordnen Sie jedes Quellfeld der entsprechenden Zielidentität zu, damit das Ziel die exportierten Kennungen erkennen und mit den vorgesehenen Benutzern verknüpfen kann.

Wählen Sie **[!UICONTROL Feld hinzufügen]** aus, um eine weitere Übereinstimmungsschlüssel-Zuordnung hinzuzufügen, oder wählen Sie das Löschsymbol aus, um eine Zuordnung zu entfernen. Überprüfen und konfigurieren Sie alle erforderlichen Zuordnungen.

Wenn die Zuordnungen abgeschlossen sind, klicken Sie auf **[!UICONTROL Weiter]**. Die geführte Einrichtung führt zum Schritt Überprüfen.

![Der Schritt Felder zuordnen , in dem die Konfiguration der Aktivierung-Übereinstimmung mit der Schlüsselzuordnung angezeigt wird.](/help/assets/destinations/manage-destinations/map-destination-fields.png)

### Überprüfung {#review-destination}

Der **[!UICONTROL Überprüfen]**-Schritt fasst die Zielkonfiguration zusammen, bevor sie erstellt wird.

Überprüfen Sie die Zieleinstellungen. Um Änderungen vorzunehmen, wählen Sie das Stiftsymbol ![Das Stiftsymbol.](../../assets/icons/edit.png) für den entsprechenden Abschnitt und aktualisieren Sie die Konfiguration.

Wenn die Konfiguration korrekt ist, wählen Sie **[!UICONTROL Abschließen]**. Das Ziel wird erstellt und steht nun zur Zielgruppenaktivierung zur Verfügung.

![Der Überprüfungsschritt, in dem die Zusammenfassung der Zielkonfiguration vor dem Abschluss angezeigt wird.](/help/assets/destinations/manage-destinations/review-destination-configuration.png)

## Anzeigen konfigurierter Ziele {#view-configured-destinations}

Nachdem Sie ein Ziel konfiguriert haben, wird es in Ihrem Zielinventar angezeigt. Aus dem Inventar können Sie den Status und die dafür aktivierten Zielgruppen überprüfen.

Navigieren Sie zu **[!UICONTROL Aktivierung]** > **[!UICONTROL Ziele]**. Auf **[!UICONTROL Registerkarte]** Ziele“ wird eine Tabelle der konfigurierten Ziele angezeigt.

![Die Registerkarte Ziele mit konfigurierten Zielen.](/help/assets/destinations/manage-destinations/configured-destinations-list.png)

## Löschen eines Ziels {#delete-destination}

Löschen eines Ziels, wenn es nicht mehr für die Zielgruppenaktivierung erforderlich ist. Wenn Sie ein Ziel löschen, wird es aus Ihrem Zielinventar entfernt und es wird verhindert, dass Zielgruppen für dieses Ziel in Zukunft aktiviert werden.

>[!IMPORTANT]
>
>Beim Löschen eines Ziels werden Zielgruppendaten, die zuvor exportiert wurden, nicht entfernt. Entfernen Sie zuvor exportierte Daten direkt aus dem Zieldatenspeicher.

Navigieren Sie zu **[!UICONTROL Aktivierung]** > **[!UICONTROL Ziele]**.

Suchen Sie das Ziel, das Sie entfernen möchten, klicken Sie auf das Auslassungssymbol in der Spalte **[!UICONTROL Aktion]** und wählen Sie dann **[!UICONTROL Löschen]** aus.

![Die Registerkarte „Ziele“ des Aktivierungsarbeitsbereichs mit dem Auslassungssymbol und der hervorgehobenen Aktion „Löschen“.](/help/assets/destinations/manage-destinations/delete-configured-destination.png)

Ein Bestätigungsdialogfeld wird angezeigt. Überprüfen Sie das Ziel, das entfernt werden soll, und wählen Sie dann **[!UICONTROL Löschen]** zur Bestätigung aus.

Das Ziel wird aus Ihrem Zielinventar entfernt und steht nicht mehr zur Zielgruppenaktivierung zur Verfügung.

## Nächste Schritte {#next-steps}

Nachdem Sie ein Ziel konfiguriert haben, können Sie mit [Aktivieren von Zielgruppen](../collaborate/activate.md) in Ihren Projekten beginnen.
