---
title: Latest Real-Time CDP Collaboration Release Notes
description: Follow the latest releases for Real-Time CDP Collaboration
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
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1461
ht-degree: 2%

---

# Latest Real-Time CDP Collaboration Release Notes

{{limited-availability-release-note}}

**Last update**: January 2026.

These release notes cover the functionality released in Adobe Real-Time CDP Collaboration. Collaboration releases operate on a continuous delivery model, which allows for an approximate monthly release cadence. These release notes get updated often, so be sure to check them regularly.

## Januar 2026 {#january-2026}

Real-Time CDP Collaboration now supports CSV file upload as a new method for sourcing audiences, as well as new mobile match keys (IDFA and GAID) for enhanced audience matching and measurement.

**Neue oder aktualisierte Funktionen**

| Funktion | Beschreibung |
| ------- | ----------- |
| CSV upload for Audience Sourcing | Upload CSV files to source audiences into Collaboration directly from the UI. Ideal for onboarding first-party data for short-term collaboration projects. For more information, see the [upload CSV file for audience sourcing guide](../setup/upload-csv-audience-sourcing.md). |
| Mobile Match Key Support | Collaboration now supports mobile match keys, including IDFA and GAID, for audience matching and measurement. These match keys are selected during account setup and can then be used when configuring connection settings for new connections and in downstream collaboration workflows. See the [Match keys setup guide](../setup/onboard-account.md#set-up-match-keys) for more details. |

{style="table-layout:auto"}

## Dezember 2025 {#december-2025}

Real-Time CDP Collaboration is now available to customers in **Europe, the Middle East, and Africa (EMEA))**. It is automatically available to Real-Time CDP Prime and Ultimate customers in these regions.

## August 2025 {#august-2025}

Real-Time CDP Collaboration is now available to customers in **Canada**. It is automatically available to Real-Time CDP Prime and Ultimate customers in these regions.

* Collaboration now supports the following [match keys](../setup/onboard-account.md#supported-match-keys):
   * Gehashte E-Mail
   * Hashed phone number
   * CRM-ID
   * Treue-ID
   * Gehashtes IPv4
   * AdFixus-ID
* Multiple match keys are now available across Collaboration, giving you the ability to expand your audience size and improve match rates. Multiple match keys can be used when sourcing audiences, establishing connections, and activating audiences. To learn more about using multiple match keys, read the [set up match keys](../setup/onboard-account.md) and [sourcing audiences](../setup/onboard-audiences.md#map-fields) guides.

>[!IMPORTANT]
>
>Beim Aktivieren von Zielgruppen, für die mehrere Übereinstimmungsschlüssel verwendet werden, schlägt die gesamte Aktivierung fehl, wenn ein (oder mehrere) Übereinstimmungsschlüssel keine Überschneidungen, keine Zielgruppengröße oder einen Schwellenwert unterschreiten. Stellen Sie vor der Aktivierung sicher, dass sich Ihre Zielgruppen ausreichend überschneiden und der Mindestschwellenwert von 1.000 IDs für alle Übereinstimmungsschlüssel erreicht wird.

* The Adobe Experience Platform destination now supports activating audiences with multiple match keys. Additionally, you can now used a linked key when configuring your destination&#39;s mapping to specify which match key is sent during activation. To learn more, read the [Experience Platform destination](../destinations/experience-platform.md#linked-keys) guide.
* Collaborators can now edit multiple audiences at once. You can now edit audience metadata, connection access, names, descriptions, and categories for multiple audiences using the bulk edit tool. To learn more about editing audiences, read the [manage audiences](../setup/onboard-audiences.md#edit-audiences) guide.

## Juli 2025 {#july-2025}

Real-time CDP Collaboration now supports brand-to-brand collaboration. Collaborators can now form connections, regardless of whether they are an advertiser or publisher. This allows for more flexible collaboration opportunities and enables brands to leverage each other&#39;s data and insights. To learn more about the differences between brand-to-brand collaboration and advertiser-to-publisher collaboration, read the [collaboration patterns](../overview/collaboration-patterns.md) guide.

* Collaborators can now connect to each other using [private connection invites](../connect/establishing-connections.md#private-connection-invites). Share your account&#39;s unique connect code with a collaborator who can then use it to connect with you directly. This is a core feature of brand-to-brand collaboration, allowing collaborators to establish connections beyond advertisers exploring the **[!UICONTROL Discover collaborators]** directory.
* [Self-serve destinations](../setup/manage-destinations.md) are now available to both advertisers and publishers.
* Audience activation is now available for both collaborators in a connection, regardless of their [account role](../overview/roles.md). Audience activation settings are configured while [establishing connections](../connect/establishing-connections.md#configure-connection-settings), allowing you to specify which collaborator can activate audiences. To learn more about audience activation, read the [activate audiences](../collaborate/activate.md) guide.
* The **[!UICONTROL Activate]** use case has been reconfigured to support brand-to-brand collaboration. The **[!UICONTROL Activate]** tab within a project now displays the audiences that have been sent to your collaborator, and the audiences activated to your destination by your collaborator. To learn more, read the [activate audiences](../collaborate/activate.md) guide. <br> ![Das Aktivierungs-Dashboard mit den Abschnitten „An Zielgruppen gesendet“ und „Aktivierte Zielgruppen“.](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* Audience-Indexwerte sind jetzt auf der Registerkarte **[!UICONTROL Entdecken]** eines Projekts verfügbar. Der Audience-Index-Wert ist ein Maß dafür, wie gut eine Zielgruppe mit der Zielgruppe Ihres Mitarbeiters übereinstimmt. Dieser Wert wird anhand der zugrunde liegenden Zielgruppengröße und Überschneidungen berechnet. Weitere Informationen zu Zielgruppenindex-Bewertungen finden Sie im Handbuch [Zielgruppenindex-Bewertung](../collaborate/discover.md#audience-index-score).

## Mai 2025 {#may-2025}

* Real-Time CDP Collaboration ist jetzt für Kunden in **Australien** und **Neuseeland** verfügbar. Sie ist für Kunden von Real-Time CDP Prime und Ultimate in diesen Regionen automatisch verfügbar.
* Real-Time CDP Collaboration bietet jetzt [Selbstbedienungsziele](../setup/manage-destinations.md) über die Registerkarte **[!UICONTROL Meine Ziele]** im Abschnitt **[!UICONTROL Setup]** an. Mit Zielen können Sie Zielgruppen in Drittanbieterplattformen wie Werbenetzwerken oder Datenverwaltungsplattformen aktivieren, um Ihre Kundinnen und Kunden über verschiedene Kanäle zu erreichen. Derzeit werden nur Adobe Experience Platform-Ziele unterstützt. Wenn Sie ein anderes Ziel konfigurieren möchten, wenden Sie sich an Ihren Adobe-Support-Mitarbeiter. Weitere Informationen zu Zielen finden Sie im Handbuch [Ziele - Übersicht](../destinations/overview.md) .
   * Ziele unterstützen auch die Anzeige von Collaboration-Zielgruppen im Zielgruppenportal [Adobe Experience Platform](https://experienceleague.adobe.com/de/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences).
* Sie können jetzt die Aktualisierungshäufigkeit der Zielgruppe für bestehende Datenverbindungen in Collaboration bearbeiten. Derzeit können Sie Ihre Zielgruppen täglich oder alle zwei bis sechs Tage aktualisieren. Weitere Informationen zum Bearbeiten der Aktualisierungshäufigkeit für Zielgruppen finden Sie im Handbuch [Datenverbindungen verwalten](../setup/manage-data-connection.md#scheduling).
* Für jeden innerhalb der Verbindung ausgewählten Anwendungsfall werden jetzt Credit-Splits zwischen Partnern festgelegt. Sie können für jeden Anwendungsfall unterschiedliche Regeln für den Kreditverbrauch festlegen, um die Verwendung Ihrer Gutschriften besser steuern zu können. Weitere Informationen zur Funktion der Kreditaufteilung finden Sie im Handbuch [Verbindungseinstellungen](../connect/establishing-connections.md#connection-settings) . Weitere Informationen zum Konsum von Guthaben finden Sie im Handbuch [Typen von &#x200B;](../setup/my-activity.md#types-of-activities)). <br> ![Bildschirm mit den Verbindungseinstellungen mit der Funktion der Kreditaufteilung.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* Publisher können jetzt Advertiser-Namen und -IDs festlegen, bevor sie die Verbindungseinstellungen von einem Advertiser akzeptieren. Publisher können Namen und IDs festlegen, die mit ihren internen Systemen übereinstimmen, die sich von den Namen und IDs des Advertisers unterscheiden können. Weitere Informationen zum Hinzufügen von Advertiser-Namen und IDs finden Sie im Handbuch [Verbindungseinstellungen](../connect/establishing-connections.md#connection-settings.md) . <br> ![Bildschirm „Verbindungseinstellungen“ mit den Herausgebereinstellungen für Advertiser-Namen und -IDs.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## April 2025 {#april-2025}

* A new **[!UICONTROL Inputs Processed]** column has been added to the credit consumption activity table. This column displays the total number of inputs (for example, IDs or rows) processed for each activity. [Read more](/help/guide/setup/my-activity.md#inputs-processed). <br> ![Inputs processed column highighted in My activity view.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* A new contact email option has been added to account creation. This helps partner collaborators reach out to you as needed during the connection process. [Weitere Informationen](../setup/onboard-account.md).

## März 2025 {#march-2025}

* When [sourcing audiences](/help/guide/setup/onboard-audiences.md) into Collaboration, you can now set an audience refresh frequency from **every one to six days** to better manage the [Audience Management credit activity](/help/guide/setup/my-activity.md#types-of-activities). For more information, read the [manage audiences](https://experienceleague.adobe.com/de/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences) guide. <br> ![Schedule screen showing different frequency intervals for updating audience membership.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "Schedule screen showing different frequency intervals for updating audience membership."){width="250" align="center" zoomable="yes"}
* When establishing a connection with a collaborator, you can now select from predefined **use cases**. The selected use case determines which project sections and product functionality become available. For more information, read the [manage projects](/help/guide/collaborate/manage-projects.md#project-use-cases) guide.
   * *Measurement* enables the **Measure** project section.
   * *Audience discovery* enables the **Discover** project section.
   * *Audience activation* enables the  **Activate** project sections <br>
* You can now delete connections with collaborators you no longer wish to work with. To learn how to delete connections, read the [deleting connections](/help/guide/connect/establishing-connections.md#delete-connections) guide.

## Februar 2025 {#february-2025}

Adobe Real-Time CDP Collaboration, purpose-built to enable advertisers and publishers to discover, activate, and measure high-value audiences without third-party cookies, is now generally available in the United States.

### Erste Schritte

1. **Access Setup**: System administrators configure access permissions for users. To learn more about configuring access permissions, read the [manage user access](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access) guide.
2. **Connect Data Sources**: Source audiences to use in Collaboration. To begin sourcing audiences, read the [source and manage audiences](/help/guide/setup/onboard-audiences.md) guide.
3. **Establish Connections**: Begin collaborating with trusted advertisers or publishers. To learn more about forming connections, read the [establishing connections](/help/guide/connect/establishing-connections.md) guide.
4. **Discover &amp; Activate**: Erstellen Sie Projekte, um wertvolle Zielgruppen zu identifizieren, die in Kampagnen aktiviert werden sollen. Weitere Informationen zum Erstellen von Projekten finden Sie im Handbuch [Verwalten &#x200B;](/help/guide/collaborate/manage-projects.md) Projekten“.

### Verfügbarkeit

* Adobe Real-Time CDP Collaboration ist derzeit nur für Kunden aus den USA verfügbar.
* Sie ist automatisch für Kunden von Adobe Real-Time CDP Prime und Ultimate verfügbar

Weitere Informationen finden Sie im Abschnitt:

* [Übersicht über Collaboration](/help/guide/home.md)
* [End-to-End-Workflow](/help/guide/overview/end-to-end-workflow.md)
* [Berechtigungen - Übersicht](/help/guide/permissions/overview.md)
