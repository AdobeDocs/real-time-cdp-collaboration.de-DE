---
title: Real-Time CDP Collaboration-Schnellstartanleitung
description: Erfahren Sie, wie Sie Ihr Unternehmen in Real-Time CDP Collaboration integrieren können, einschließlich der Einrichtung von Rollen und Organisationen, der Beschaffung von Zielgruppen, der Aktivierung und Messung. Dieser Leitfaden hilft Mitarbeitern bei der Konfiguration von Verbindungseinstellungen, um mit der sicheren und effizienten Nutzung ihrer Zielgruppen zu beginnen.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 68e5095e-ece5-4f64-9056-10f3b216cf0c
source-git-commit: ac8db9f5a3879d548d8dc3818ad20fc602b31e7c
workflow-type: tm+mt
source-wordcount: '1408'
ht-degree: 0%

---

# Real-Time CDP Collaboration-Schnellstartanleitung

{{limited-availability-release-note}}

Beginnen Sie mit Real-Time CDP Collaboration, indem Sie Ihr Unternehmen konfigurieren, Zielgruppen finden und eine datenschutzorientierte Aktivierung und Messung aktivieren.

## Voraussetzungen

Bevor Sie beginnen, stellen Sie Folgendes sicher:

- Eine aktive Real-Time CDP Collaboration-Lizenz.
- [System- oder Produktadministratorzugriff auf Adobe Experience Platform](./permissions/overview.md).
- [Zugriff für Endbenutzer bereitgestellt](./permissions/manage-user-access.md).
- [Für Ihr Unternehmen erstellte und Benutzern zugewiesene Rollen](./permissions/manage-roles.md).
- Zugriff auf Branding-Assets, z. B. Name, Logo und Banner Ihres Unternehmens.
- Eine [definierte Strategie für Übereinstimmungsschlüssel](./setup/onboard-account.md#set-up-match-keys) (derzeit ist die Hash-E-Mail der einzige unterstützte Übereinstimmungsschlüssel).
- (Optional) Zugriff auf eine unterstützte Cloud-Quelle (Amazon S3 oder Snowflake), wenn Sie Experience Platform nicht für die Zielgruppenverwaltung verwenden.

## Schritt 1: Rollenbasierte Einrichtung abschließen {#complete-role-based-setup}

Die Zugriffsrollen Ihres Unternehmens bestimmen, was Benutzende in Collaboration sehen und tun können. Bevor Sie fortfahren, stellen Sie sicher, dass rollenbasierte Berechtigungen korrekt eingerichtet sind, um den entsprechenden Zugriff und die Sichtbarkeit in der Plattform sicherzustellen.

**Ressourcen:**

- [Dokumentation zum Benutzerzugriff](./permissions/manage-user-access.md)
- [Dokumentation zur Rolleneinrichtung](./permissions/manage-roles.md)


Sehen Sie sich dieses Video an, um zu erfahren, wie Sie Produktzugriff und Berechtigungen für Collaboration mithilfe von Admin Console und Experience Platform zuweisen.

>[!VIDEO](https://video.tv.adobe.com/v/3452239/?learn=on&enablevpops&captions=ger)

## Schritt 2: Einrichten des Collaboration-Kontos {#set-up-your-account}

Bevor Sie Zielgruppen beziehen können, müssen Sie Ihr -Konto in Collaboration konfigurieren. Dies legt fest, wie Sie in der Benutzeroberfläche angezeigt werden und worauf Sie Zugriff haben.

Wenn Sie nicht über den erforderlichen Zugriff verfügen, gehen Sie zurück zu Schritt 1 oder wenden Sie sich an den Administrator Ihrer Organisation, um Hilfe beim Durchführen dieser Einrichtung zu erhalten.

Definieren Sie die Rolle Ihres Kontos in Collaboration, stellen Sie Branding-Assets bereit und konfigurieren Sie Übereinstimmungsschlüssel, um Zielgruppen über Verbindungen hinweg auszurichten.

>[!NOTE]
>
>Sie können während der Einrichtung ein oder mehrere Konten erstellen (z. B. einen Advertiser und einen Publisher). Bestimmte Felder wie Branding-Assets und Kontakt-E-Mails können später im Arbeitsbereich **[!UICONTROL Einstellungen]** aktualisiert werden.

- **Rolle zuweisen** - Bestimmt, ob Ihr Konto ein Advertiser oder ein Publisher ist. Ihre Rolle definiert, welche Funktionen Sie in Collaboration haben. Weitere Informationen dazu, wie sich Rollen auf den Workflow für die Zusammenarbeit auswirken, finden Sie im Handbuch [Rollen](./overview/roles.md) .
- **Branding-**: Fügen Sie Ihrem Konto Folgendes hinzu:
   - Kontoname (max. 100 Zeichen)
   - Beschreibung (max. 1.000 Zeichen)
   - Logo (SVG &lt;20KB, idealerweise quadratisch)

>[!NOTE]
>
>Wenn Sie ein Publisher-Konto erstellen und im Verbindungskatalog von Collaboration öffentlich angezeigt werden möchten, wenden Sie sich an Ihren Adobe-Kundenbetreuer. Für Publisher-Konten ist ein benutzerdefiniertes Markenbanner erforderlich (JPG 2688x1536). Diese Datei kann direkt mit Ihrem Kundenbetreuer geteilt werden.

- **Kontakt-E** - Geben Sie eine Geschäfts-E-Mail an, die Mitarbeiter nach der Herstellung einer Verbindung verwenden können.
- **Übereinstimmungsschlüssel konfigurieren** - Wählen Sie die Kennungen aus, die für den Zielgruppen-Abgleich verwendet werden (derzeit ist die gehashte E-Mail der einzige unterstützte Übereinstimmungsschlüssel).

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
- **Aktualisierungen planen** - Definieren der Aktualisierungshäufigkeit (z. B. täglich).
- **Einverständniseinstellungen konfigurieren** - Bestimmen Sie, welche Profile für die Aufnahme in Verbindungen infrage kommen, indem Sie einen Einverständnismodus auswählen: Opt-in, Opt-out oder Ohne.

>[!NOTE]
>
>Sie können Zielgruppen hinzufügen oder entfernen und den Aktualisierungszeitplan direkt in Collaboration aktualisieren. Um andere Einstellungen wie Übereinstimmungsschlüssel oder Einverständnismodus zu ändern, müssen Sie die Datenverbindung löschen und neu erstellen.

>[!IMPORTANT]
>
>**Maximale Anzahl von Zielgruppen pro Rolle des Mitarbeiters:**
>
>- **Werbetreibende** können bis zu 25 Zielgruppen beziehen.
>- **Publisher** können bis zu 250 Zielgruppen (mit jeweils mindestens 1.000 IDs) beschaffen.

>[!IMPORTANT]
>
>**Wesentliche Anforderungen erfüllen:**
>
>Alle Übereinstimmungsschlüssel müssen **trimmed**, **lowercase** und **SHA256-hashed** sein.\
>Wenn Sie Hash-Werte mit Großbuchstaben angeben, wandelt Collaboration diese automatisch in Kleinbuchstaben um.\
>Wenn Ihre Quelle (**)** enthält, verwenden Sie die Option **[!UICONTROL Umwandlung anwenden]** zum Anwenden von Hashing. Diese Option ist nur verfügbar, wenn Zielgruppen aus Experience Platform bezogen werden, und wird für Cloud-basierte Quellen nicht unterstützt.
>
>Weitere Informationen finden Sie im Abschnitt [Zuordnungsfelder](./setup/onboard-audiences.md#map-fields) des Handbuchs für die Quell- und Zielgruppenverwaltung.

Sehen Sie sich das folgende Video an, um eine vollständige exemplarische Vorgehensweise zur Quelle von Zielgruppen mit Collaboration anzuzeigen.

>[!VIDEO](https://video.tv.adobe.com/v/3452217/?learn=on&enablevpops)

Alternativ finden Sie weitere Informationen im Dokument [Sourcing von Zielgruppen in Collaboration](./setup/onboard-audiences.md#source-and-manage-audiences).

### Option B: Source von Snowflake oder Amazon S3

Um eine Cloud-Quelle zu konfigurieren (z. B. [!DNL AWS S3] oder [!DNL Snowflake]), bereiten Sie Ihre Zielgruppendaten mit der folgenden [Zielgruppenspezifikations-PDF&quot; ](../assets/quick-start/RTCDP_Collaboration_Audience_Onboarding_Spec_v1.0.pdf). Wenden Sie sich nach Abschluss des Vorgangs oder bei Fragen an Ihren Adobe-Kundenbetreuer, um die Einrichtung abzuschließen. Diese Methode ist kein Self-Service und erfordert die Unterstützung von Adobe.

>[!IMPORTANT]
>
>Cloud-basierte Zielgruppendateien müssen dem erforderlichen Schema entsprechen, das in der PDF für Zielgruppenspezifikationen beschrieben ist. Dateien müssen Hash-Kennungen (kleinbuchstabierte SHA256), erforderliche Metadatenfelder wie `segment_name` und `activation_id` enthalten und unterstützte Formate wie CSV oder Parquet verwenden. Adobe normalisiert Daten nicht vor der Aktivierung. TTL wird basierend auf der Lebensdauer der Zielgruppe erzwungen.
>
>Alle Zielgruppen in der hochgeladenen Datei werden zu diesem Zeitpunkt vollständig bezogen. Die [Einstellung für die Zielgruppensichtbarkeit](/help/guide/setup/onboard-audiences.md#metadata-visibility) bestimmt, ob Ihre Mitarbeiter Ihre Zielgruppe anzeigen können, und wird über die Collaboration-Benutzeroberfläche verwaltet.

## Schritt 4: Aktivieren von Zielgruppen (für Experience Platform oder ein Cloud-Ziel) {#activate-audiences}

Aktivieren Sie als Nächstes Zielgruppen entweder für Ihre Experience Platform-Instanz oder für ein Cloud-Ziel.

### Option A: Für Experience Platform aktivieren

Führen Sie die folgenden Schritte aus, die im Handbuch [Konfigurieren von Adobe Experience Platform als Ziel](/help/guide/destinations/experience-platform.md) beschrieben sind.

- **Ziel erstellen** - Verwenden Sie die Benutzeroberfläche zum Einrichten eines Experience Platform-Ziels (Sandbox-Ebene).
- **Map-Übereinstimmungsschlüssel** - Wählen Sie die Kennung aus (z. B. `hashedEmail`).
- **TTL definieren** - Gültigkeit festlegen (1-30 Tage).
- **Überprüfen in Zielgruppenportal** - Nachdem ein Mitarbeiter Ihnen eine Zielgruppe gesendet hat, überprüfen Sie, ob sie im Zielgruppenportal unter der Herkunft &quot;[!UICONTROL Real-Time CDP Collaboration&quot; &#x200B;].

### Option B: Für Cloud aktivieren

Um ein Cloud-Ziel zu konfigurieren (z. B. [!DNL AWS S3] oder [!DNL Snowflake]), wenden Sie sich an Ihren Adobe-Kundenbetreuer, um den Einrichtungsprozess zu starten. Je nach Cloud-Ziel müssen Sie Cloud-Zieldetails wie Dateipfad, Anmeldeinformationen, Konto-Locators usw. angeben. Sobald die erforderlichen Informationen bereitgestellt wurden, konfiguriert Adobe das Cloud-Ziel-Setup.

Zielgruppendaten, die an ein Cloud-Ziel gesendet werden, folgen einem vordefinierten Schema. Eine ausführliche Beschreibung der erforderlichen Felder und des Formats finden Sie im [Collaboration Audience Activation-Handbuch](../assets/quick-start/RTCDP_Collaboration_Audience_Activation_Spec_v1.0.pdf).

## Schritt 5: Einrichten der Messung (optional) {#set-up-measurement}

>[!AVAILABILITY]
>
>Diese Funktion befindet sich in **Beta** und steht nur Kunden mit eingeschränkter Verfügbarkeit zur Verfügung. Wenden Sie sich an den Adobe-Support, um Zugriff zu erhalten.

>[!IMPORTANT]
>
>Der **[!UICONTROL Measure]**-Arbeitsbereich ist nur verfügbar, wenn der **[!UICONTROL Measurement]**-Anwendungsfall [während des Verbindungsprozesses](./connect/establishing-connections.md#connection-settings) aktiviert wurde. Weitere Informationen zu Anwendungsfällen finden Sie im Handbuch [Verwalten von ](./collaborate/manage-projects.md#project-use-cases)&quot;.

Collaboration bietet eine Vielzahl von Berichten zur Analyse der Reichweite, Häufigkeit und Effektivität von Kampagnen. Der Arbeitsbereich **[!UICONTROL Kennzahlen]** ist zwar in der Benutzeroberfläche verfügbar, die vollständige Reporting-Funktionalität erfordert jedoch möglicherweise eine Backend-Aktivierung.

Informationen zum Anzeigen und Interpretieren von Messberichten finden Sie im [Messhandbuch](./collaborate/measure.md). Es behandelt Attribution, zusammengefasste Kampagnenmetriken und Dashboards wie Reichweitenkurven und Häufigkeitsverteilung.

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

## Schritt 6: Vernetzung mit Partnern {#connect-with-collaborators}

Nach Abschluss des Setups ist Ihr Unternehmen nun bereit, sich mit Partnern zu verbinden, indem Einladungen gesendet oder angenommen und Projekteinstellungen zur Genehmigung eingereicht werden. Dieser Verbindungsprozess umfasst das Senden oder Empfangen von Einladungen, das Überprüfen und Senden von Verbindungseinstellungen (z. B. Anwendungsfälle und Kreditverbrauch) und das Bestätigen der Verbindung.

Verwenden Sie als Advertiser den Arbeitsbereich **[!UICONTROL Verbinden]** im linken Navigationsmenü, um verfügbare Publisher zu durchsuchen. Alternativ können sich Mitarbeiter über (private [) direkt miteinander ](./connect/establishing-connections.md#private-connection-invite){target="_blank"}.

>[!NOTE]
>
>Derzeit können nur Werbetreibende Herausgeber durchsuchen. Publisher können keine Verbindungen zu Advertisern suchen oder initiieren.

Einen Überblick über diesen Fluss finden Sie im [Handbuch zum Herstellen von Verbindungen](./connect/establishing-connections.md){target="_blank"}. Eine visuelle Anleitung zum Verbindungsprozess, einschließlich dem Durchsuchen von Partnern und dem Verwalten von Verbindungseinstellungen, finden Sie im Video [Einrichten von Advertiser-Konten](https://experienceleague.adobe.com/de/docs/platform-learn/tutorials/collaboration/connect-with-publishers){target="_blank"}.

## Nächste Schritte

Sie haben jetzt die Ersteinrichtung abgeschlossen und Ihr Unternehmen für eine sichere Zusammenarbeit konfiguriert. Erkunden Sie als Nächstes die folgenden Ressourcen, um Ihr Verständnis von Aktivierung, Messung und Data Governance zu vertiefen:

- [Dokumentation zum Workflow für die Zielgruppenaktivierung](./collaborate/activate.md)
- [Anwendungsfälle für Messungen](./collaborate/measure.md)
- [Best Practices für die Collaboration-Governance](./setup/onboard-audiences.md#governance-policy-and-enforcement-actions)
