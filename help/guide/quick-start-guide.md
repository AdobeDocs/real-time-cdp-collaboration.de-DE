---
title: Schnellstart für das Real-Time CDP Collaboration-Onboarding
description: Erfahren Sie, wie Sie Ihr Unternehmen in Real-Time CDP Collaboration integrieren können, einschließlich der Einrichtung von Rollen und Organisationen, der Bereitstellung, Aktivierung und Messung von Audiences. Dieses Handbuch hilft Werbetreibenden und Publishern, die Einstellungen für die Zusammenarbeit zu konfigurieren und mit der sicheren und effizienten Verwendung freigegebener Zielgruppen zu beginnen.
audience: admin, publisher, advertiser
source-git-commit: 4435788917dd82cb127525e054f7f09803e1dcdf
workflow-type: tm+mt
source-wordcount: '1595'
ht-degree: 0%

---

# Schnellstart für das Real-Time CDP Collaboration-Onboarding

Beginnen Sie mit Real-Time Customer Data Platform (CDP) Collaboration, indem Sie Ihre Organisation konfigurieren, Zielgruppen bereitstellen und eine datenschutzorientierte Aktivierung und Messung aktivieren.

## Voraussetzungen

Bevor Sie beginnen, stellen Sie Folgendes sicher:

- Eine aktive Real-Time CDP Collaboration-Lizenz.
- [System- oder Produktadministratorzugriff auf Adobe Experience Platform](./permissions/overview.md#use-cases).
- [Zugriff für Endbenutzer bereitgestellt](./permissions/manage-user-access.md).
- [Für Ihr Unternehmen erstellte und Benutzern zugewiesene Rollen](./permissions/manage-roles.md).
- Zugriff auf Branding-Assets, z. B. Name, Logo und Banner Ihres Unternehmens.
- Eine [definierte Strategie für Übereinstimmungsschlüssel](./setup/onboard-organization.md#set-up-match-keys) (derzeit ist die Hash-E-Mail der einzige unterstützte Übereinstimmungsschlüssel).
- (Optional) Zugriff auf eine unterstützte Cloud-Quelle (Amazon S3 oder Snowflake), wenn Sie Experience Platform nicht als Ziel verwenden.

## Schritt 1: Rollenbasierte Einrichtung abschließen {#complete-role-based-setup}

>[!NOTE]
>
>Dieser Schritt gilt sowohl für Werbetreibende als auch für Herausgeber.

Die Zugriffsrollen Ihres Unternehmens bestimmen, was Benutzende in Real-Time CDP Collaboration sehen und tun können. Bevor Sie fortfahren, stellen Sie sicher, dass rollenbasierte Berechtigungen korrekt eingerichtet sind, um den entsprechenden Zugriff und die Sichtbarkeit in der Plattform sicherzustellen.

**Ressourcen:**

- [Dokumentation zum Benutzerzugriff](./permissions/manage-user-access.md)
- [Dokumentation zur Rolleneinrichtung](./permissions/manage-roles.md)


Sehen Sie sich dieses Video an, um zu erfahren, wie Sie Produktzugriff und Berechtigungen für Collaboration über die Benutzeroberfläche von Admin Console und Experience Platform zuweisen.

>[!VIDEO](https://video.tv.adobe.com/v/3452216/?learn=on&enablevpops)

## Schritt 2: Einrichten der Real-Time CDP Collaboration-Organisation {#set-up-your-organization}

>[!NOTE]
>
>Dieser Schritt gilt sowohl für Werbetreibende als auch für Herausgeber.

Bevor Sie Zielgruppen hinzufügen können, müssen Sie Ihr Unternehmen in Collaboration konfigurieren. Dies bestimmt, wie Ihre Organisation in der Benutzeroberfläche angezeigt wird und sich verhält.

Wenn Sie keinen Administratorzugriff auf Experience Platform haben, wenden Sie sich an den Administrator Ihres Unternehmens, um Hilfe beim Durchführen dieser Einrichtung zu erhalten.

Definieren Sie die Rolle Ihres Unternehmens in Collaboration, stellen Sie Branding-Assets bereit und konfigurieren Sie Übereinstimmungsschlüssel, um Zielgruppen über Verbindungen hinweg auszurichten. Führen Sie dann die folgenden Schritte aus, um die Einrichtung abzuschließen und Ihr Unternehmen für die Interaktion mit Ihren Verbindungen vorzubereiten.

>[!NOTE]
>
>Sie können während der Einrichtung einen oder mehrere Mitarbeiter erstellen (z. B. Advertiser- oder Publisher-Profile). Bestimmte Felder wie Branding-Assets und Kontakt-E-Mails können später im Arbeitsbereich **[!UICONTROL Einstellungen]** aktualisiert werden. Übereinstimmungsschlüssel können auf Projektebene entfernt, aber nicht hinzugefügt werden. Daher sollten sie sorgfältig geplant werden.

- **Rolle zuweisen** - Legt fest, ob Ihr Unternehmen als Advertiser, Publisher oder beides fungiert. Ihre Rolle definiert, welche Kooperationsfunktionen Sie haben, z. B. die Freigabe von Zielgruppen (Advertiser) initiieren oder Zielgruppen verfügbar machen (Publisher). Weitere Informationen dazu, wie sich Rollen auf den Workflow für die Zusammenarbeit auswirken, finden [ im Handbuch zum End-to-End-Workflow ](./end-to-end-workflow.md).
- **Branding-**: Fügen Sie Ihrem Konto Folgendes hinzu:
   - Markenname (max. 100 Zeichen)
   - Markenbezeichnung (max. 1.000 Zeichen)
   - Markenlogo (SVG &lt;20 KB, idealerweise quadratisch)
   - Markenbanner (JPG 2688x1536 oder ähnlich)
- **Kontakt-E** - Geben Sie eine Geschäfts-E-Mail an, die Mitarbeiter nach der Herstellung einer Verbindung verwenden können.

  >[!NOTE]
  >
  >Wenn Sie ein Herausgeberkonto erstellen und im Verbindungskatalog von Collaboration öffentlich sichtbar sein möchten, wenden Sie sich an Ihren Adobe-Kundenbetreuer. Für Publisher-Konten ist ein benutzerdefiniertes Markenbanner erforderlich (JPG 2688x1536). Diese Datei kann direkt mit Ihrem Kundenbetreuer geteilt werden.

- **Übereinstimmungsschlüssel konfigurieren** - Wählen Sie die Kennungen aus, die für den Zielgruppen-Abgleich verwendet werden (derzeit ist die gehashte E-Mail der einzige unterstützte Übereinstimmungsschlüssel).

Sobald Ihre Organisation erstellt und Ihre Branding- und Übereinstimmungsschlüssel konfiguriert sind, kann Ihre Organisation mit der Bereitstellung von Zielgruppen und der Aktivierung von Daten beginnen.

Weitere Informationen zur Ersteinrichtung der Organisation, einschließlich der Definition von Rollen, dem Hochladen von Branding-Assets und der Konfiguration von Übereinstimmungsschlüsseln, finden Sie im Dokument [Ersteinrichtung der Organisation](./setup/onboard-organization.md#initial-organization-setup){target="_blank"}.

Sehen Sie sich eine schrittweise Anleitung zur Einrichtung von Advertisern an, einschließlich Kontoerstellung, Branding und Konfiguration von Übereinstimmungsschlüsseln.

>[!VIDEO](https://video.tv.adobe.com/v/3452264/?learn=on&enablevpops)

## Schritt 3: Source-Zielgruppen (aus Experience Platform oder einer Cloud-Quelle) {#source-audiences}

Wählen Sie einen oder beide der folgenden Datenspeicher aus, um Zielgruppen zu beziehen. Verwenden Sie entweder die Collaboration-Benutzeroberfläche oder stimmen Sie sich mit Adobe ab, um Zielgruppen in einem datenschutzkonformen Format bereitzustellen.

### Option A: Source aus Experience Platform

[Verwenden Sie die Benutzeroberfläche der Collaboration-Ziele, um eine Sandbox zu verknüpfen, die Zielgruppen enthält](./setup/onboard-audiences.md). Verwenden Sie diese Self-Service-Methode, um auf vorhandene Zielgruppensegmente in Ihrer Experience Platform-Instanz zu verweisen.

### Option B: Source von Snowflake oder Amazon S3

Um eine Cloud-Quelle zu konfigurieren (z. B. [!DNL AWS S3] oder [!DNL Snowflake]), bereiten Sie Ihre Zielgruppendaten mit der folgenden [Zielgruppenspezifikations-PDF&quot; ](../assets/quick-start/RTCDP_Collaboration_Audience_Onboarding_Spec_v1.0.pdf). Wenden Sie sich nach Abschluss des Vorgangs oder bei Fragen an Ihren Adobe-Kundenbetreuer, um die Einrichtung abzuschließen. Diese Methode ist kein Self-Service und erfordert die Unterstützung von Adobe.

>[!IMPORTANT]
>
>Cloud-basierte Zielgruppendateien müssen dem erforderlichen Schema entsprechen, das in der PDF für Zielgruppenspezifikationen beschrieben ist. Dateien müssen Hash-Kennungen (kleinbuchstabierte SHA256), erforderliche Metadatenfelder wie `segment_name` und `activation_id` enthalten und unterstützte Formate wie CSV oder Parquet verwenden. Adobe normalisiert Daten nicht vor der Aktivierung. TTL wird basierend auf der Lebensdauer der Zielgruppe erzwungen.
>
>Alle Zielgruppen in der hochgeladenen Datei werden zu diesem Zeitpunkt vollständig bezogen. Der Zugriff auf bestimmte Partnerorganisationen wird separat über die Collaboration-Benutzeroberfläche bereitgestellt.

### Bereitstellen von Audiences

Konfigurieren Sie, wie Zielgruppen für die Verwendung in Verbindungen vorbereitet, abgeglichen und gesteuert werden.

- **Zielgruppen auswählen** *(nur Experience Platform)* - Zielgruppensegmente mit unterstützten Kennungen auswählen.
- **Übereinstimmungsschlüssel zuordnen**: Die Zielgruppenfelder werden an den konfigurierten Übereinstimmungsschlüsseln ausgerichtet.
- **Umwandlungen anwenden** - Nur-Text-Werte (z. B. E-Mail) bei Bedarf hashen.
- **Aktualisierungen planen** - Definieren der Aktualisierungshäufigkeit (z. B. täglich).
- **Einverständniseinstellungen konfigurieren** - Bestimmen Sie, welche Profile für die Aufnahme in Verbindungen infrage kommen, indem Sie einen Einverständnismodus auswählen: Opt-in, Opt-out oder Ohne.

>[!NOTE]
>
>Sie können Zielgruppen hinzufügen oder entfernen und den Aktualisierungszeitplan direkt in der Collaboration-Benutzeroberfläche aktualisieren. Um andere Einstellungen wie Übereinstimmungsschlüssel oder Einverständnismodus zu ändern, müssen Sie die Datenverbindung löschen und neu erstellen.

>[!IMPORTANT]
>
>**Maximale Anzahl von Zielgruppen pro Rolle des Mitarbeiters:**
>
>- **Werbetreibende** können bis zu 25 Zielgruppen bereitstellen.
>- **Publisher** können bis zu 250 Zielgruppen bereitstellen (jede mit mindestens 5.000 IDs).

>[!IMPORTANT]
>
>**Wesentliche Anforderungen erfüllen:**
>
>Alle Übereinstimmungsschlüssel müssen **trimmed**, **lowercase** und **SHA256-hashed** sein.\
>Wenn Sie Hash-Werte mit Großbuchstaben angeben, wandelt Collaboration diese automatisch in Kleinbuchstaben um.\
>Wenn Ihre Quelle (**)** enthält, verwenden Sie die Option **[!UICONTROL Umwandlung anwenden]** in der Benutzeroberfläche, um Hashing anzuwenden. Diese Option ist nur verfügbar, wenn Zielgruppen aus Experience Platform bezogen werden, und wird für Cloud-basierte Quellen nicht unterstützt.
>
>Weitere Informationen finden Sie im Abschnitt [Zuordnungsfelder](./setup/onboard-audiences.md#map-fields) des Handbuchs zum Importieren und Verwalten von Audiences.

Eine vollständige exemplarische Vorgehensweise zum Referenzieren von Zielgruppen mithilfe der Collaboration-Benutzeroberfläche finden Sie im folgenden Demonstrationsvideo zu Collaboration-Zielgruppen-Referenzen .

>[!VIDEO](https://video.tv.adobe.com/v/3452217/?learn=on&enablevpops)

Alternativ finden Sie weitere Informationen im Dokument [Verfügbarmachen von Zielgruppen in Real-Time CDP Collaboration](https://experienceleague.adobe.com/en/docs/real-time-cdp-collaboration/using/setup/onboard-audiences#import-audiences).

## Schritt 4: Aktivieren von Zielgruppen (für Experience Platform oder ein Cloud-Ziel) {#activate-audiences}

>[!NOTE]
>
>Dieser Schritt gilt sowohl für Werbetreibende als auch für Herausgeber.

Verwenden Sie die Collaboration-Benutzeroberfläche, um Zielgruppen für Ihre Experience Platform-Instanz oder ein Cloud-Ziel zu aktivieren.

### Option A: Für Experience Platform aktivieren

Führen Sie die folgenden Schritte aus, die im Handbuch [Konfigurieren von Adobe Experience Platform als Ziel](https://experienceleague.adobe.com/en/docs/real-time-cdp-collaboration/using/destinations/experience-platform) beschrieben sind.

- **Ziel erstellen** - Verwenden Sie die Benutzeroberfläche zum Einrichten eines Experience Platform-Ziels (Sandbox-Ebene).
- **Map-Übereinstimmungsschlüssel** - Wählen Sie die Kennung aus (z. B. `hashedEmail`).
- **TTL definieren** - Gültigkeit festlegen (1-30 Tage).
- **Überprüfen in Zielgruppenportal** - Nachdem ein Mitarbeiter Ihnen eine Zielgruppe gesendet hat, überprüfen Sie, ob sie im Zielgruppenportal unter der Herkunft &quot;[!UICONTROL Real-Time CDP Collaboration&quot; &#x200B;].

### Option B: Für Cloud aktivieren

Um Zielgruppen für ein Cloud-Ziel zu aktivieren (z. B. [!DNL AWS S3] oder [!DNL Snowflake]), wenden Sie sich an Ihren Adobe-Kundenbetreuer, um den Einrichtungsprozess zu starten. Sie müssen Zieldetails wie Dateipfad, Anmeldeinformationen und das erwartete Dateiformat angeben. Während des Setups müssen Sie auch einen Übereinstimmungsschlüssel angeben (z. B. `hashedEmail`) und die gewünschte TTL und Aktualisierungskadenz definieren. Sobald die Konfiguration abgeschlossen ist, stellt Adobe das Ziel bereit und stellt sicher, dass die Daten korrekt bereitgestellt werden.

Zielgruppendaten, die an ein Cloud-Ziel gesendet werden, folgen einem vordefinierten Schema. Eine ausführliche Beschreibung der erforderlichen Felder und des Formats finden Sie im [Collaboration Audience Activation-Handbuch](../assets/quick-start/RTCDP_Collaboration_Audience_Activation_Spec_v1.0.pdf).

### Die wichtigsten Unterschiede

In der folgenden Liste sind die Unterschiede zwischen Experience Platform- und Cloud-Aktivierungsoptionen aufgeführt:

- Aktivierungen für Experience Platform erfolgen vollständig im Selbstbedienungsmodus und sind im Zielgruppenportal sichtbar.
- Cloud-Ziele erfordern eine Adobe-Koordinierung und werden nicht in der Benutzeroberfläche angezeigt.

## Schritt 5: Einrichten der Messung (optional) {#set-up-measurement}

>[!AVAILABILITY]
>
>Diese Funktion befindet sich in **Beta** und steht nur Kunden mit eingeschränkter Verfügbarkeit zur Verfügung. Wenden Sie sich an den Adobe-Support, um Zugriff zu erhalten.

>[!IMPORTANT]
>
>Der **[!UICONTROL Measure]**-Arbeitsbereich ist nur verfügbar, wenn der **[!UICONTROL Measurement]**-Anwendungsfall [während des Verbindungsprozesses](./connect/establishing-connections.md#connection-settings) aktiviert wurde. Weitere Informationen zu Anwendungsfällen finden Sie im Handbuch [Verwalten von ](./collaborate/manage-projects.md#project-use-cases)&quot;.

Collaboration bietet eine Vielzahl von Berichten zur Analyse der Reichweite, Häufigkeit und Effektivität von Kampagnen. Der Arbeitsbereich **[!UICONTROL Kennzahlen]** ist zwar in der Benutzeroberfläche verfügbar, die vollständige Reporting-Funktionalität erfordert jedoch möglicherweise eine Backend-Aktivierung.

Informationen zum Anzeigen und Interpretieren von Messberichten finden Sie im [Messhandbuch](./collaborate/measure.md). Es behandelt Attribution, zusammengefasste Kampagnenmetriken und Dashboards wie Reichweitenkurven und Häufigkeitsverteilung.

<!-- Commenting out the below information as this workflow is not yet in Beta but will be imminently. A guided measurement configuration workflow will be available in a future release."
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
   - Submit the report. It will run on the selected date and populate within 24 hours. -->

## Verifizierung

Überprüfen Sie nach der Aktivierung, ob Zielgruppen im entsprechenden Ziel erfolgreich bereitgestellt oder bereitgestellt wurden.

- Stellen Sie sicher, dass Ihre Zielgruppen im Zielgruppen-Portal angezeigt werden (für die Experience Platform-Aktivierung).
- Bestätigen Sie die erfolgreiche Cloud-Bereitstellung über externe Zielprotokolle oder eine Bestätigung.

## Schritt 6: Vernetzung mit Partnern {#connect-with-collaborators}

Nach Abschluss der Einrichtung und der Datenbereitstellung kann Ihr Unternehmen nun mit Partnern in Kontakt treten, indem Einladungen gesendet oder angenommen und Projekteinstellungen zur Genehmigung eingereicht werden. Dieser Verbindungsprozess umfasst das Senden oder Empfangen von Einladungen, das Überprüfen und Senden von Verbindungseinstellungen (z. B. Anwendungsfälle und Kreditverbrauch) und das Bestätigen der Beziehung.

Verwenden Sie den **[!UICONTROL Verbinden]**-Arbeitsbereich über das linke Navigationsmenü in der Collaboration-Benutzeroberfläche, um verfügbare Publisher zu durchsuchen (Advertiser können derzeit nicht durchsucht werden). Einen Überblick über diesen Fluss finden Sie im [Handbuch Verbinden mit Werbetreibenden oder Herausgebern](./connect/establishing-connections.md){target="_blank"}. Eine visuelle Anleitung zum Verbindungsprozess, einschließlich dem Durchsuchen von Partnern und dem Verwalten von Verbindungseinstellungen, finden Sie im Video [Einrichten von Advertiser-Konten](https://experienceleague.adobe.com/de/docs/platform-learn/tutorials/collaboration/connect-with-publishers){target="_blank"}.

## Nächste Schritte

Sie haben jetzt das Onboarding abgeschlossen und Ihr Unternehmen für eine sichere Zusammenarbeit konfiguriert. Erkunden Sie als Nächstes die folgenden Ressourcen, um Ihr Verständnis von Aktivierung, Messung und Data Governance zu vertiefen:

- [Dokumentation zum Workflow für die Zielgruppenaktivierung](./collaborate/activate.md)
- [Anwendungsfälle für Messungen](./collaborate/measure.md)
- [Best Practices für die Collaboration-Governance](./setup/onboard-audiences.md#governance-policy-and-enforcement-actions)
