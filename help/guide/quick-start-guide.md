---
title: Real-Time CDP Collaboration Quick Start & Setup Guide
description: Erfahren Sie, wie Sie Real-Time CDP Collaboration einrichten, Rollen und Konten konfigurieren, Zielgruppen identifizieren, Daten aktivieren und eine sichere Verbindung mit Partnern herstellen können.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 68e5095e-ece5-4f64-9056-10f3b216cf0c
TQID: https://experienceleague.adobe.com/rhIArZZm0Thkj3E-qiHtVHO6qxpr1vd-Qs4hWt4tf1U
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1417
ht-degree: 2%

---

# Real-Time CDP Collaboration quick start guide

{{limited-availability-release-note}}

Get started with Real-Time CDP Collaboration by configuring your organization, sourcing audiences, and enabling privacy-focused activation and measurement.

## Voraussetzungen

Before you begin, ensure you have the following:

- An active Real-Time CDP Collaboration license.
- [System or product administrator access to Adobe Experience Platform](./permissions/overview.md).
- [Access provisioned for end users](./permissions/manage-user-access.md).
- [Roles created for your organization and assigned to users](./permissions/manage-roles.md).
- Access to branding assets, such as your organization&#39;s name, logo, and banner.
- A [defined match key strategy](./setup/onboard-account.md#set-up-match-keys)
- (Optional) Access to a supported cloud source (Amazon S3, Google Cloud Storage, or Snowflake) if you&#39;re not using Experience Platform for audience management.

## Step 1: Complete role-based setup {#complete-role-based-setup}

Your organization&#39;s access roles determine what users can see and do in Collaboration. Before proceeding, make sure role-based permissions are set up correctly to ensure appropriate access and visibility in the platform.

**Resources:**

- [User Access Documentation](./permissions/manage-user-access.md)
- [Role Setup Documentation](./permissions/manage-roles.md)


Watch this video to learn how to assign product access and permissions for Collaboration using the Admin Console and Experience Platform.

>[!VIDEO](https://video.tv.adobe.com/v/3452239/?captions=ger&learn=on&enablevpops)

## Step 2: Set up your Collaboration account {#set-up-your-account}

Before you can source audiences, you must configure your account in Collaboration. This governs how you appear and what you have access to in the interface.

If you don&#39;t have the necessary access, please refer back to step 1 or contact your organization&#39;s administrator for help completing this setup.

Define your account&#39;s role in Collaboration, provide branding assets, and configure match keys to align audiences across connections.

>[!NOTE]
>
>You can create one or more accounts (such as advertiser and a publisher) during setup. Bestimmte Felder wie Branding-Assets und Kontakt-E-Mails können später im Arbeitsbereich **[!UICONTROL Einstellungen]** aktualisiert werden.

- **Rolle zuweisen** - Bestimmt, ob Ihr Konto ein Advertiser oder ein Publisher ist. Ihre Rolle definiert, welche Funktionen Sie in Collaboration haben. Weitere Informationen dazu, wie sich Rollen auf den Workflow für die Zusammenarbeit auswirken, finden Sie im Handbuch [Rollen](./overview/roles.md) .
- **Branding-**: Fügen Sie Ihrem Konto Folgendes hinzu:
   - Kontoname (max. 100 Zeichen)
   - Beschreibung (max. 1.000 Zeichen)
   - Logo (SVG &lt;20KB, idealerweise quadratisch)

>[!NOTE]
>
>Wenn Sie ein Publisher-Konto erstellen und im Verbindungskatalog von Collaboration öffentlich angezeigt werden möchten, wenden Sie sich an Ihren Adobe-Kundenbetreuer. Für Publisher-Konten ist ein benutzerdefiniertes Markenbanner erforderlich (JPG 2688x1536). Diese Datei kann direkt mit Ihrem Kundenbetreuer geteilt werden.

- **Kontakt-E** - Geben Sie eine Geschäfts-E-Mail an, die Mitarbeiter nach der Herstellung einer Verbindung verwenden können.
- **Übereinstimmungsschlüssel konfigurieren** - Wählen Sie die Kennungen aus, die für den Zielgruppen-Abgleich verwendet werden.

Weitere Informationen zur Ersteinrichtung von Konten, einschließlich der Definition von Rollen, dem Hochladen von Branding-Assets und dem Konfigurieren von Übereinstimmungsschlüsseln, finden Sie im Handbuch [Ersteinrichtung von Konten](./setup/onboard-account.md#initial-account-setup){target="_blank"} .

In diesem Video erhalten Sie eine schrittweise Anleitung zur Einrichtung von Advertisern, einschließlich Kontoerstellung, Branding und Konfiguration von Übereinstimmungsschlüsseln.

>[!VIDEO](https://video.tv.adobe.com/v/3452264/?learn=on&enablevpops)

## Schritt 3: Source-Zielgruppen (aus Experience Platform oder einer Cloud-Quelle) {#source-audiences}

Sobald Ihr Konto erstellt und Ihre Branding- und Übereinstimmungsschlüssel konfiguriert sind, können Sie mit der Beschaffung von Zielgruppen beginnen. Wählen Sie je nach Datenspeicher und Geschäftsanforderungen eine der folgenden Beschaffungsmethoden.

### Option A: Source aus Experience Platform

[Verwenden Sie Collaboration, um eine Sandbox zu verknüpfen, die Zielgruppen enthält](./setup/onboard-audiences.md). Verwenden Sie diese Self-Service-Methode, um auf vorhandene Zielgruppensegmente in Ihrer Experience Platform-Instanz zu verweisen.

#### Audiences konfigurieren

Konfigurieren Sie, wie Zielgruppen für die Verwendung in Verbindungen vorbereitet, abgeglichen und gesteuert werden.

- **Zielgruppen auswählen** *(nur Experience Platform)* - Zielgruppensegmente mit unterstützten Kennungen auswählen.
- **Übereinstimmungsschlüssel zuordnen**: Die Zielgruppenfelder werden an den konfigurierten Übereinstimmungsschlüsseln ausgerichtet.
- **Umwandlungen anwenden** - Nur-Text-Werte (z. B. E-Mail) bei Bedarf hashen.
- **Schedule refreshes** – Define update frequency (for example, daily).
- **Configure consent settings** – Determine which profiles are eligible to be included in connections by selecting a consent mode: opt-in, opt-out, or none.

>[!NOTE]
>
>You can add or remove audiences and update the refresh schedule directly in Collaboration. To change other settings, such as match keys or consent mode, you must delete and recreate the data connection.

>[!IMPORTANT]
>
>**Maximum number of audiences per collaborator role:**
>
>- **Advertisers** can source up to 25 audiences.
>- **Publishers** can source up to 250 audiences (each with a minimum of 1,000 IDs).

>[!IMPORTANT]
>
>**Match key requirements:**
>
>All match keys must be **trimmed**, **lowercased**
>Hash-Übereinstimmungsschlüssel müssen **SHA256-hashed** sein.\
>Wenn Sie Hash-Werte mit Großbuchstaben angeben, wandelt Collaboration diese automatisch in Kleinbuchstaben um.\
>If your source contains **plaintext identifiers**, use the **[!UICONTROL Apply transformation]** option to apply hashing. Diese Option ist nur verfügbar, wenn Zielgruppen aus Experience Platform bezogen werden, und wird für Cloud-basierte Quellen nicht unterstützt.
>
>For more information, see the [map fields](./setup/onboard-audiences.md#map-fields) section of the source and manage audiences guide.

To see a full walkthrough of how to source audiences using Collaboration, watch the video below.

>[!VIDEO](https://video.tv.adobe.com/v/3452217/?learn=on&enablevpops)

Alternatively, see the document on [sourcing audiences in Collaboration](./setup/onboard-audiences.md#source-and-manage-audiences).

### Option B: Source from Snowflake, Amazon S3, or Google Cloud Storage

To configure a cloud source, such as [!DNL Snowflake], [!DNL Amazon S3], or [!DNL Google Cloud Storage], prepare your audience data using the [Audience Specification PDF](../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf)

You can configure [!DNL Amazon S3], [!DNL Google Cloud Storage], or [!DNL Snowflake] as self-service data sources. For setup instructions, see the [Amazon S3 sourcing guide](./setup/configure-aws-s3-audience-sourcing.md), the [GCS sourcing guide](./setup/configure-gcs-audience-sourcing.md), or the [Snowflake sourcing guide](./setup/configure-snowflake-audience-sourcing.md).

For other cloud service providers, contact your Adobe account representative to finalize the setup.

>[!IMPORTANT]
>
>Cloud-based audience files must follow the required schema outlined in the Audience Specification PDF. Files must include hashed identifiers (lowercased SHA256), required metadata fields such as `segment_name` and `activation_id`, and use supported formats such as CSV or Parquet. Adobe does not normalize data before activation. TTL is enforced based on the audience&#39;s lifespan.
>
>All audiences in the uploaded file are fully sourced at this stage. The [audience visibility setting](/help/guide/setup/onboard-audiences.md#metadata-visibility) determines whether your collaborators can view your audience and is managed through the Collaboration UI.

## Step 4: Activate audiences (to Experience Platform or a cloud destination) {#activate-audiences}

Next, activate audiences to either your Experience Platform instance or a cloud destination.

### Option A: Activate to Experience Platform

Complete the following steps outlined in the [configure Adobe Experience Platform as a destination](/help/guide/destinations/experience-platform.md) guide.

- **Create a destination** – Use the UI to set up an Experience Platform destination (sandbox-level).
- **Map match keys** – Select the identifier (e.g., `hashedEmail`).
- **Define TTL** – Set expiration (1–30 days).
- **Verify in Audience Portal** – Once a collaborator sends you an audience, verify that it appears in the Audience Portal under the origin &quot;[!UICONTROL Real-Time CDP Collaboration].&quot;

### Option B: Activate to cloud

To configure a cloud destination (for example, [!DNL AWS S3] or [!DNL Snowflake]), contact your Adobe account representative to initiate the setup process. Depending on the cloud destination, you will need to provide cloud destination details such as file path, credentials, account locators etc. Once required information is provided, Adobe will configure the cloud destination setup.

Audience data sent to a cloud destination follows a predefined schema. For a detailed description of the required fields and format, download the [Collaboration Audience Activation Guide](../assets/quick-start/RTCDP_Collaboration_Audience_Activation_Spec_v1.0.pdf).

## Step 5: Set up measurement (optional) {#set-up-measurement}

>[!IMPORTANT]
>
>The **[!UICONTROL Measure]** workspace is only available if the **[!UICONTROL Measurement]** use case was enabled [during the connection process](./connect/establishing-connections.md#connection-settings). Weitere Informationen zu Anwendungsfällen finden Sie im Handbuch [Verwalten von &#x200B;](./collaborate/manage-projects.md#project-use-cases)&quot;.

Collaboration offers a variety of reports to analyze campaign reach, frequency, and effectiveness. While the **[!UICONTROL Measure]** workspace is available in the UI, full reporting functionality may require backend enablement.

To learn how to view and interpret measurement reports, see the [Measurement guide](./collaborate/measure.md). It covers attribution, campaign summary metrics, and dashboards such as reach curves and frequency distribution.

<!-- 
Commenting out the below information as this workflow is not yet in Beta but will be imminently. A guided measurement configuration workflow will be available in a future release."

### Configure measurement workflow

Collaboration supports two measurement workflows:

- **Attribution using Adobe Experience Platform datasets**
- **Campaign summary using only partner-provided data**

Choose the appropriate workflow below based on your campaign measurement goals.

#### Option A: Attribution using Experience Platform datasets

Use this workflow to measure conversion activity using datasets stored in Experience Platform.

1. **Create a measurement data connection**
   - Select the dataset that contains your conversion events.
   - Map identity fields from your dataset to the match keys used in Collaboration.
   - Manage consent and governance settings.
   - Define one or more conversion events to measure.
   - Review and confirm your setup.

2. **Run a measurement report**
   - Go to the **[!UICONTROL Measure]** workspace within the associated project.
   - Input the report name, date range, and report run date.
   - Select **[!UICONTROL Attribution]** as the report type.
   - Select the defined conversion event(s).
   - Submit the report. It will run on the specified date and populate within 24 hours.

#### Option B: Campaign summary using partner-provided data

Use this workflow to generate campaign summary insights based on advertiser-supplied identifiers (for example, campaign ID).

1. **Set up the connection**
   - In the connection settings, ensure **[!UICONTROL Measurement]** is selected as a use case.
   - Create a project under the connection with **[!UICONTROL Measurement]** as an activity.

2. **Provide campaign context**
   - Input required campaign identifiers (for example, **Campaign ID**) for the partner to reference.
   - Align with your partner on campaign scope and reporting timeline.

3. **Run a measurement report**
   - Navigate to the **[!UICONTROL Measure]** workspace within the project.
   - Input the report name, date range, and report run date.
   - Select **[!UICONTROL Campaign summary]** as the report type.
   - Submit the report. It will run on the selected date and populate within 24 hours. 
-->

## Step 6: Connect with collaborators {#connect-with-collaborators}

With setup complete, your organization is now ready to connect with collaborators by sending or accepting invitations and submitting project settings for approval. This connection process involves sending or receiving invitations, reviewing and submitting connection settings (such as use cases and credit consumption), and confirming the connection.

Verwenden Sie als Advertiser den Arbeitsbereich **[!UICONTROL Verbinden]** im linken Navigationsmenü, um verfügbare Publisher zu durchsuchen. Alternativ können sich Mitarbeiter über (private [) direkt miteinander &#x200B;](./connect/establishing-connections.md#private-connection-invite){target="_blank"}.

>[!NOTE]
>
>Derzeit können nur Werbetreibende Herausgeber durchsuchen. Publisher können keine Verbindungen zu Advertisern suchen oder initiieren.

Einen Überblick über diesen Fluss finden Sie im [Handbuch zum Herstellen von Verbindungen](./connect/establishing-connections.md){target="_blank"}. Eine visuelle Anleitung zum Verbindungsprozess, einschließlich dem Durchsuchen von Partnern und dem Verwalten von Verbindungseinstellungen, finden Sie im Video [Einrichten von Advertiser-Konten](https://experienceleague.adobe.com/de/docs/platform-learn/tutorials/collaboration/connect-with-publishers){target="_blank"}.

## Nächste Schritte

Sie haben jetzt die Ersteinrichtung abgeschlossen und Ihr Unternehmen für eine sichere Zusammenarbeit konfiguriert. Erkunden Sie als Nächstes die folgenden Ressourcen, um Ihr Verständnis von Aktivierung, Messung und Data Governance zu vertiefen:

- [Dokumentation zum Workflow für die Zielgruppenaktivierung](./collaborate/activate.md)
- [Anwendungsfälle für Messungen](./collaborate/measure.md)
- [Best Practices für die Collaboration-Governance](./setup/onboard-audiences.md#governance-policy-and-enforcement-actions)
