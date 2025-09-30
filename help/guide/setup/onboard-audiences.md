---
title: Source und Verwalten von Audiences
description: Erfahren Sie, wie Sie Zielgruppen in Adobe Real-Time CDP Collaboration beschaffen und verwalten.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: 36f43d9d34ce7851a1c7093e0891f9c87e56387c
workflow-type: tm+mt
source-wordcount: '3508'
ht-degree: 16%

---

# Source und Verwalten von Audiences

{{limited-availability-release-note}}

Zielgruppen sind spezifische Benutzergruppen oder Kundinnen bzw. Kunden, die anhand verschiedener Attribute segmentiert werden. Diese ermöglichen es den Mitarbeitern, bei zielgerichteten Marketing- und personalisierten Erlebnissen zusammenzuarbeiten, um effektivere Werbekampagnen zu ermöglichen. In diesem Handbuch wird beschrieben, wie Sie Zielgruppen in Real-Time CDP Collaboration beschaffen, das Zielgruppen-Dashboard anzeigen und einzelne Zielgruppen verwalten.

## Source-Zielgruppen in Collaboration {#source-audiences}

>[!IMPORTANT]
>
>Um Zielgruppen beziehen zu können, muss den Benutzenden eine Rolle zugewiesen werden, die zwei Profilverwaltungsberechtigungen enthält: **[!UICONTROL Profile anzeigen]** und **[!UICONTROL Segmente]**. Informationen zum Zuweisen der erforderlichen Berechtigungen finden Sie im Handbuch [Zielgruppen-Beschaffung](../permissions/overview.md#audience-sourcing) unter Berechtigungen.

Bevor Sie Zielgruppen mit Partnern aktivieren und Überschneidungsberechnungen durchführen können, müssen die Zielgruppen in Collaboration bezogen werden. Um Zielgruppen zu beziehen, befolgen Sie die Workflow-Schritte im folgenden Abschnitt.

Wählen Sie im Arbeitsbereich **[!UICONTROL Setup]** **[!UICONTROL auf der Registerkarte „Meine Zielgruppen]** das Symbol zum Hinzufügen (![Hinzufügen) aus.](/help/assets/icons/plus.png)) und wählen Sie dann **[!UICONTROL Audience]** aus. Wenn dies Ihre erste Zielgruppe ist, können Sie auch die Option **[!UICONTROL Hinzufügen] auswählen**.

![Mein Zielgruppen-Arbeitsbereich mit hervorgehobener Option „Hinzufügen“ und hervorgehobener Option „Zielgruppen“.](/help/assets/setup/add-manage-audiences/add-audiences.png){zoomable="yes"}

### Auswählen der Datenverbindung {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="Marketing-Aktionen"
>abstract="<p>Verwenden Sie Marketing-Aktionen, um zu steuern, welche Zielgruppendaten aus Experience Platform in Real-Time CDP Collaboration importiert werden sollen. Die Marketing-Aktion <strong>Data Collaboration</strong> unterstützt Datennutzungs-Labels vom Typ C4, C5 und C9. Die Marketing-Aktion <strong>Datenwissenschaft</strong> unterstützt das Datennutzungs-Label vom Typ C9.</p> <p> <ul><li> Wenn das Kontrollkästchen <em>aktiviert</em> ist, werden alle mit den oben genannten Labels in Experience Platform markierten Daten, ausgeschlossen und <strong>nicht</strong> in Real-Time CDP Collaboration übertragen.</li><li> Wenn das Kontrollkästchen <em>deaktiviert</em> ist, gibt es keine Einschränkung für Daten aus Experience Platform, die in Real-Time CDP Collaboration importiert werden können.</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=de" text="Datennutzungs-Labels – Übersicht"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html?lang=de" text="Glossar der Datennutzungs-Labels"

>[!IMPORTANT]
>
>Nachdem Sie Ihre erste Datenverbindung hergestellt und Ihre erste Zielgruppe abgerufen haben, können Sie mehrere Zielgruppen aus der vorhandenen Datenverbindung beziehen. Beim Hinzufügen zusätzlicher Zielgruppen beginnen Sie mit dem Schritt [Zielgruppe auswählen](#select-audiences), da die Datenverbindung bereits hergestellt wurde.

Eine Datenverbindung ist die Datenquelle, aus der Sie Zielgruppen beziehen. Derzeit wird nur Adobe Experience Platform als Datenverbindung unterstützt.

Alle Einstellungen, die Sie für Ihre Datenverbindung konfigurieren, werden auf alle Zielgruppen angewendet, die von dieser Datenverbindung bezogen werden.

>[!TIP]
>
>Es gibt einen separaten Workflow, in dem Sie Ihre Datenverbindungen anzeigen und bearbeiten können. Weitere Informationen finden Sie im [Verwalten von Datenverbindungen](/help/guide/setup/manage-data-connection.md).

Um mit dem Hinzufügen Ihrer Datenverbindung zu beginnen, wählen Sie **[!UICONTROL Neue Datenverbindung hinzufügen]** und dann **[!UICONTROL Weiter]** aus.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit hervorgehobener Option „Neue Datenverbindung hinzufügen“.](/help/assets/setup/add-manage-audiences/add-data-connection.png){zoomable="yes"}

#### Datenquelle auswählen

Als Nächstes wählen Sie die Quelle für Ihre Datenverbindung. Zu den verfügbaren Quellen gehören:

* **Adobe Experience Platform**: Wählen Sie diese Option, um Ihre Zielgruppen aus Adobe Experience Platform einzubringen.
* **CSV-Datei** (künftige Version): Laden Sie eine CSV-Datei hoch, die Ihre Zielgruppendaten enthält, um Daten schnell und einfach aufzunehmen.
* **Amazon Web Services** (zukünftige Version): Stellen Sie eine Verbindung zu Ihrem Amazon S3-Speicher her, um Zielgruppendaten direkt aus Ihren S3-Buckets zu beziehen.
* **Snowflake** (zukünftige Version): Verwenden Sie Ihr Snowflake Data Warehouse, um Zielgruppendaten nahtlos abzurufen.
* **Google Cloud Platform** (zukünftige Version): Stellen Sie eine Verbindung zu Ihrem Google Cloud-Speicher her, um Zielgruppendaten direkt aus Ihren GCS-Buckets zu beziehen.

Wählen Sie Ihre Datenquelle und dann **[!UICONTROL Weiter]** aus.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit hervorgehobener Option &quot;Adobe Experience Platform&quot;.](/help/assets/setup/add-manage-audiences/select-data-connection-source.png){zoomable="yes"}

#### Sandbox auswählen

Nachdem Sie Ihre Datenquelle ausgewählt haben, müssen Sie die Sandbox auswählen, die die Zielgruppen enthält, die Sie für Collaboration verwenden möchten. Wählen Sie die Sandbox aus der Liste der verfügbaren Sandboxes aus und klicken Sie dann auf **[!UICONTROL Weiter]**

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit ausgewählter Sandbox.](/help/assets/setup/add-manage-audiences/select-sandbox.png){zoomable="yes"}

#### Governance-Richtlinie und Durchsetzungsmaßnahmen {#governance-policy-and-enforcement-actions}

Als Nächstes müssen Sie sicherstellen, dass für die Quelldaten die richtigen Marketing-Aktionen festgelegt sind. Sie müssen außerdem der Verwendung von Daten aus Experience Platform für die Datenerfassung zustimmen.

Verwenden Sie Marketing-Aktionen, um zu steuern, welche Zielgruppendaten aus Experience Platform in Collaboration importiert werden sollen. Die Marketing-Aktion **[!UICONTROL Data Collaboration]** unterstützt Datennutzungs-Labels vom Typ C4, C5 und C9. Die Marketing-Aktion **[!UICONTROL Datenwissenschaft]** unterstützt das Datennutzungs-Label vom Typ C9.

Lesen Sie mehr über die [C4-, C5- und C9-Datennutzungskennzeichnungen](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}.

* Wenn das Kontrollkästchen ***aktiviert*** wird, werden alle Daten, die wie oben beschrieben in Experience Platform gekennzeichnet sind, ausgeschlossen und **nicht** in Collaboration importiert.
* Wenn das Kontrollkästchen ***deaktiviert*** aktiviert ist, gibt es keine Einschränkung für Daten, die aus Experience Platform bezogen werden.

Weitere Informationen zu Datennutzungskennzeichnungen finden Sie in der Dokumentation zu Experience Platform:

* [Datennutzungs-Labels – Übersicht](https://experienceleague.adobe.com/de/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [Glossar zu Datennutzungskennzeichnungen](https://experienceleague.adobe.com/de/docs/experience-platform/data-governance/labels/reference){target="_blank"}

Darüber hinaus sollten Sie Ihre Einverständnisregeln auswählen, die auf Daten angewendet werden, die in Collaboration bezogen werden.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ im Abschnitt „Governance-Richtlinie und Durchsetzungsaktionen“.](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png){zoomable="yes"}

Nachdem Sie die Marketing-Aktionen und Einverständnisregeln ausgewählt haben, klicken Sie auf **[!UICONTROL Weiter]**, um mit dem nächsten Schritt fortzufahren. Es erscheint ein Bestätigungsdialogfeld, in dem Sie aufgefordert werden, die Bedingungen zu akzeptieren. Aktivieren Sie das Kontrollkästchen und klicken Sie dann zur Bestätigung **[!UICONTROL OK]**.

![Das Dialogfeld „Governance-Richtlinie“ und „Durchsetzungsaktionen“ mit hervorgehobenem Kontrollkästchen und hervorgehobener Option „OK“.](/help/assets/setup/add-manage-audiences/data-collaboration-consent-confirmation.png){zoomable="yes"}

### Details angeben

Geben Sie als Nächstes einen Namen und eine Beschreibung für Ihre Datenverbindung an. Diese Informationen helfen Ihnen später bei der Identifizierung der Datenverbindung.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit der Option, einen Namen und eine Beschreibung anzugeben.](/help/assets/setup/add-manage-audiences/data-connection-details.png){zoomable="yes"}

### Zuordnen von Feldern {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="Quellfelder"
>abstract="Quellfelder sind Identity-Namespaces und Attribute aus Ihrer Implementierung von Experience Platform. Sie können diese Zielfeldern zuordnen, die in Collaboration definiert sind."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="Zielfelder"
>abstract="Zielfelder sind die Übereinstimmungsschlüssel, die bei der Kontoeinrichtung ausgewählt wurden. Standardmäßig sind alle ausgewählten Übereinstimmungsschlüssel verfügbar."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="Transformation anwenden"
>abstract="Verwenden Sie beim Beziehen von Feldern *ohne Hash* diese Option, damit Collaboration den Hash anwendet und die einfachen Felder in Hash-Felder umwandelt."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_identity_namespaces"
>title="Identity-Namespaces"
>abstract="Wählen Sie einen Identity-Namespace aus den standardmäßigen und benutzerdefinierten Identity-Namespaces aus, die in Ihrer Experience Platform-Organisation verfügbar sind."
>additional-url="https://experienceleague.adobe.com/de/docs/experience-platform/identity/features/namespaces#standard" text="Standardmäßige und Identity-Namespaces in Experience Platform"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_profile_attributes"
>title="Profilattribute"
>abstract="Wählen Sie Attribute aus dem Vereinigungsschema für die Klasse „Profile“ in Experience Platform aus. Diese Ansicht zeigt Attribute an, die im Vereinigungsschema vorhanden sind und zur Klasse „XDM-Profil für Kontakt“ gehören."
>additional-url="https://experienceleague.adobe.com/de/docs/experience-platform/profile/union-schemas/union-schema" text="Vereinigungsschema in Experience Platform"

Als Nächstes wählen Sie Quellfelder aus, die Zielfeldern in Collaboration zugeordnet werden sollen. Die verfügbaren Zielfelder basieren auf den Übereinstimmungsschlüsseln, die Sie bei der Kontoeinrichtung ausgewählt haben.

>[!IMPORTANT]
>
>Derzeit können Sie Datenverbindungen nicht bearbeiten, um neue Zuordnungsfelder einzuschließen. Wenn Sie Ihrem Konto neue Übereinstimmungsschlüssel hinzufügen, nachdem Ihre Datenverbindung erstellt wurde, müssen Sie eine neue Datenverbindung erstellen, um sie zuzuordnen.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit der Option, Quellfelder Zielfeldern zuzuordnen.](/help/assets/setup/add-manage-audiences/add-map-fields.png){zoomable="yes"}

>[!TIP]
>
>Sie können demselben Zielfeld mehrere Quellfelder zuordnen. Wenn sich beispielsweise E-Mail-Adressen in zwei separaten Feldern in Experience Platform befinden, können Sie diese jeweils dem Zielfeld **[!UICONTROL gehashte E-Mail]** als zwei separate Zeilen zuordnen. Verwenden Sie die Option **[!UICONTROL Feld hinzufügen]**, um zusätzliche Zuordnungszeilen hinzuzufügen.

>[!BEGINSHADEBOX]

**[!UICONTROL Source-Felder]** sind Identitäts-Namespaces und -Attribute aus Experience Platform. Dazu gehören sowohl [standardmäßige](https://experienceleague.adobe.com/de/docs/experience-platform/identity/features/namespaces#standard){target="_blank"} als [benutzerdefinierte](https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html#create-namespaces){target="_blank"} Identitäts-Namespaces. Sie enthalten auch Profilattribute, die im [Vereinigungsschema“ vorhanden sind ](https://experienceleague.adobe.com/de/docs/experience-platform/profile/union-schemas/union-schema){target="_blank"} zur Klasse „XDM Individual Profile“ gehören.

Source-Felder werden den in Collaboration definierten Zielfeldern zugeordnet.

**[!UICONTROL Zielfelder]** geben an, wie die Identitäten in Collaboration referenziert werden. Zielfelder sind die Übereinstimmungsschlüssel, die bei der Kontoeinrichtung ausgewählt wurden. Standardmäßig sind alle ausgewählten Übereinstimmungsschlüssel verfügbar.

Verwenden Sie die **[!UICONTROL Umwandlung anwenden]**, wenn Sie (*gehashte) Felder* Hash-Feldern beziehen. Collaboration wendet den Hash an und wandelt die Felder um. Der von Adobe verwendete Hash-Algorithmus ist SHA256.

>[!ENDSHADEBOX]

Um mit der Zuordnung von Feldern zu beginnen, wählen Sie das leere Quellfeld neben dem Zielfeld aus. Das **[!UICONTROL Quellfeld auswählen]** wird angezeigt. Wählen Sie zwischen den **[!UICONTROL Identity-]**) und **[!UICONTROL Profilattribute]**, um das gewünschte Quellfeld zu finden, und wählen Sie dann das Feld aus der Liste aus. Sie können auch die Suchoption verwenden, um das gewünschte Feld zu finden.

![Das Dialogfeld „Quellfeld auswählen“ mit den angezeigten E-Mail-Optionen.](/help/assets/setup/add-manage-audiences/select-source-field.png){zoomable="yes"}

Um die Beschaffung eines nicht gehashten Felds in ein gehashtes Zielfeld zu verarbeiten, verwenden Sie die Option **[!UICONTROL Umwandlung anwenden]**. Um beispielsweise ein zweites E-Mail-Feld hinzuzufügen, wählen Sie die Option **[!UICONTROL Feld hinzufügen]** aus, um eine neue Zeile hinzuzufügen, und wählen Sie dann **[!UICONTROL gehashte E-Mail]** für das Zielfeld aus. Wählen Sie ein nicht gehashtes E-Mail-Quellfeld aus und dann **[!UICONTROL Umwandlung anwenden]**.

![Der Arbeitsbereich Zielgruppen hinzufügen mit den E-Mail-Quellfeldern, die dem Zielfeld zugeordnet sind, wobei Umwandlung anwenden für ein Feld aktiviert ist.](/help/assets/setup/add-manage-audiences/apply-transformation.png){zoomable="yes"}

Fügen Sie für jedes Zielfeld weitere Zuordnungspaare hinzu. Wenn Sie keinen Übereinstimmungsschlüssel verwenden möchten, können Sie ihn mithilfe des Löschsymbols (![Löschsymbol](/help/assets/icons/delete.png)) neben dem Feld entfernen. Wenn der Übereinstimmungsschlüssel entfernt wird, kann er nicht mehr zum Abrufen von Zielgruppen aus der Verbindung verwendet werden.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit hervorgehobener Option „Löschen“ neben einem Zielfeld.](/help/assets/setup/add-manage-audiences/remove-target-field.png){zoomable="yes"}

Wenn Sie mit dem Zuordnen von Feldern fertig sind, wählen Sie **[!UICONTROL Weiter]** aus, um fortzufahren.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit ausgefüllten Zuordnungsfeldern und hervorgehobener Option „Weiter“.](/help/assets/setup/add-manage-audiences/confirm-field-mapping.png){zoomable="yes"}

### Zeitplan {#schedule}

Als Nächstes planen Sie, wann die Zielgruppen gefüllt werden sollen. Die Zielgruppe wird gemäß diesem Zeitplan aktualisiert.

![Der Arbeitsbereich „Zielgruppe hinzufügen“ mit den angezeigten Planungsoptionen.](/help/assets/setup/add-manage-audiences/audience-scheduling.png){zoomable="yes"}

>[!IMPORTANT]
>
>Durch die Anpassung der Aktualisierungshäufigkeit der Zielgruppe können Sie die [Audience-Management-](/help/guide/setup/my-activity.md#types-of-activities)&quot; verwalten, die pro Zielgruppenaktualisierung berechnet wird. Die Auswahl einer höheren Häufigkeit kann sich auf die Aktualität der Daten auswirken, die für Zielgruppen-Discover-Berichte und die Zielgruppen-Aktivierung verfügbar sind.

Wählen Sie aus der Dropdown-Liste „Häufigkeit“ die Häufigkeit **[!UICONTROL Aktualisierung]** Zielgruppe aus.

![Der Arbeitsbereich Zielgruppen-Planung hinzufügen mit geöffnetem Dropdown-Menü „Häufigkeit“.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png){zoomable="yes"}

Wählen Sie anschließend den **[!UICONTROL Datumsbereich]** aus. Das Startdatum ist das Datum, an dem die Zielgruppe mit Profilen befüllt wird. Das Enddatum ist, an dem die Aktualisierung der Zielgruppe beendet wird.

![Die Option Zielgruppen hinzufügen im Planungsarbeitsbereich mit Datumsbereich wird angezeigt.](/help/assets/setup/add-manage-audiences/audience-scheduling-date-range.png){zoomable="yes"}

>[!IMPORTANT]
>
>Nach dem Enddatum im Datumsbereich werden alle Zielgruppen, die von dieser Datenverbindung bezogen werden, nicht mehr aktualisiert. Um die Verbindung zu erneuern, folgen Sie der Anleitung [Datenverbindung verwalten](/help/guide/setup/manage-data-connection.md).

### Zielgruppen auswählen {#select-audiences}

Nach Auswahl der Zielgruppenquelle wählen Sie bestimmte Zielgruppen aus, die einbezogen werden sollen. Verwenden Sie die Such- und Filteroptionen, um die relevanten Zielgruppen aus Ihrer Datenverbindung zu finden. Wählen Sie die gewünschten Zielgruppen aus und klicken Sie dann auf **[!UICONTROL Weiter]**.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit einer Liste verfügbarer Zielgruppen.](/help/assets/setup/add-manage-audiences/select-audience.png){zoomable="yes"}

### Überprüfung

Überprüfen Sie alle Konfigurationen und Einstellungen, bevor Sie das Hinzufügen der Zielgruppe abschließen. Stellen Sie sicher, dass alle Details korrekt sind, und wählen Sie **[!UICONTROL Abschließen]** aus, um die Erstellung Ihrer Datenverbindung abzuschließen.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit allen ausgewählten Konfigurationen wird angezeigt.](/help/assets/setup/add-manage-audiences/review-connection.png){zoomable="yes"}

## Anzeigen des Dashboards „Zielgruppen“ {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="Fehlende Identitäten"
>abstract="Die Anzahl der Identitäten ist nach der nächsten Aktualisierung der Datenverbindung gemäß dem konfigurierten Zeitplan verfügbar. Die erste Aktualisierung erfolgt normalerweise innerhalb von 24 Stunden nach der Einrichtung der Datenverbindung. Laufende Aktualisierungen folgen dem konfigurierten Zeitplan."

Nach der Beschaffung von Zielgruppen zeigt der **[!UICONTROL Meine Zielgruppen]** Arbeitsbereich alle Zielgruppen an, die derzeit in Collaboration bezogen werden.

![Der Arbeitsbereich „Meine Zielgruppen“ mit allen aus der Quelle stammenden Zielgruppen.](/help/assets/setup/add-manage-audiences/audiences-workspace.png)

Jede Zielgruppe enthält einen Überblick über die folgenden Informationen:

| Element | Beschreibung |
|----------|---------|
| **[!UICONTROL Name]** | Der Name der Zielgruppe. |
| **[!UICONTROL Identitäten]** | Gibt die Anzahl der in dieser Zielgruppe vorhandenen Identitäten an. Beachten Sie Folgendes: Wenn dasselbe Profil zwei oder mehr Identitäten hat und diese Identitäten als Übereinstimmungsschlüssel im Projekt verwendet werden, wird das Profil zweimal in der Zählung angezeigt. |
| **[!UICONTROL Status]** | Gibt an, ob die Zielgruppe aktiv ist und in Projekten verwendet werden kann. Der Status **[!UICONTROL Ausstehend]** gibt an, dass die Zielgruppe gerade erst abgerufen wurde und Identitäten noch ausgefüllt werden müssen. Die Zielgruppen der Quelle werden nach der ersten Aktualisierung, die in der Regel innerhalb von 24 Stunden nach der Einrichtung der Datenverbindung erfolgt, mit Profilen gefüllt. |
| **[!UICONTROL Quelle]** | Gibt an, woher die Zielgruppe stammt. In der aktuellen Version von Collaboration ist Experience Platform die einzige unterstützte Quelle. |
| **[!UICONTROL Datenverbindung]** | Die Datenverbindung, von der die Zielgruppe stammt. Sie können den Namen auswählen, um die Datenverbindung anzuzeigen. |
| **[!UICONTROL Verbindungszugriff]** | Definiert, ob die Zielgruppe privat oder öffentlich ist. Öffentliche Zielgruppen sind in Überschneidungsberichten auffindbar und können innerhalb eines Projekts aktiviert werden. |
| **[!UICONTROL Erstellt]** | Gibt an, wann die Zielgruppe ursprünglich in Collaboration aufgenommen wurde. |
| **[!UICONTROL Zuletzt aktualisiert]** | Gibt das letzte Datum und die letzte Uhrzeit der Aktualisierung der Zielgruppe in Collaboration an. Dies bezieht sich nicht auf den Zeitpunkt der letzten Aktualisierung der Zielgruppe, sondern auf den Zeitpunkt der letzten Änderung der Konfiguration oder der Metadaten der Zielgruppe. |

![Der Arbeitsbereich Meine Zielgruppe mit allen aus der Quelle stammenden Zielgruppen.](/help/assets/setup/add-manage-audiences/audiences-workspace.png){zoomable="yes"}

Um Schnellaktionen für eine Zielgruppe durchzuführen, klicken Sie auf die **mit den Auslassungspunkten…** neben dem Namen der Zielgruppe. Die folgenden Optionen sind verfügbar:

* **[!UICONTROL Kategorien bearbeiten]** ermöglicht das Hinzufügen verschiedener Kategorie-Tags zur Audience. Weitere Informationen finden Sie im Abschnitt [Kategorien](#categories) unten.
* **[!UICONTROL Löschen]** wird die Zielgruppe aus der Datenverbindung gelöscht.

![Der Arbeitsbereich „Meine Zielgruppen“ mit geöffnetem Menü und hervorgehobenen Optionen „Kategorien bearbeiten“ und „Löschen“.](/help/assets/setup/add-manage-audiences/audiences-ellipsis-menu.png){zoomable="yes"}

## Anzeigen einzelner Zielgruppen {#view-individual-audiences}

Um Informationen für eine einzelne Zielgruppe anzuzeigen und zu aktualisieren, wählen Sie die Zielgruppe im Arbeitsbereich **[!UICONTROL Meine Zielgruppen]** aus. Der Zielgruppen-Arbeitsbereich zeigt detaillierte Informationen zur ausgewählten Zielgruppe an, einschließlich Details, Identitäten, Kategorien, Verbindungszugriff und Einstellungen für die Sichtbarkeit von Metadaten.

### Zielgruppendetails

Für jede einzelne Zielgruppe werden die folgenden Informationen angezeigt:

| Element | Beschreibung |
|----------|---------|
| **[!UICONTROL Status]** | Gibt an, ob die Zielgruppe aktiv ist und in Projekten verwendet werden kann. |
| **[!UICONTROL Quelle]** | Gibt an, woher die Zielgruppe stammt. In der aktuellen Version von Collaboration ist Experience Platform die einzige unterstützte Quelle. |
| **[!UICONTROL Datenverbindung]** | Die Datenverbindung, von der die Zielgruppe stammt. |
| **[!UICONTROL Zuletzt aktualisiert]** | Gibt das letzte Datum und die letzte Uhrzeit der Aktualisierung der Zielgruppe in Collaboration an. Dies bezieht sich nicht auf den Zeitpunkt der letzten Aktualisierung der Zielgruppe, sondern auf den Zeitpunkt der letzten Änderung der Konfiguration oder der Metadaten der Zielgruppe |
| **[!UICONTROL Zuletzt aktualisiert von]** | Gibt den Benutzer an, der die Zielgruppe zuletzt aktualisiert hat. |
| **[!UICONTROL Erstellt]** | Gibt an, wann die Zielgruppe ursprünglich in Collaboration aufgenommen wurde. |
| **[!UICONTROL Erstellt von]** | Gibt den Benutzer an, der die Zielgruppe in Collaboration aufgenommen hat. |

![Arbeitsbereich einer einzelnen Zielgruppe.](/help/assets/setup/add-manage-audiences/audience-details.png){zoomable="yes"}

#### Identitäten {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="Identitäten"
>abstract="Eine Aufschlüsselungsansicht der Identitäten, aus denen diese Zielgruppe besteht, getrennt durch Übereinstimmungsschlüssel."

Der **[!UICONTROL Identitäten]** gibt die Anzahl der in der Zielgruppe vorhandenen Identitäten an. Der Abschnitt enthält auch eine Aufschlüsselung der Identitäten nach Übereinstimmungsschlüssel, anhand derer Sie die Zusammensetzung der Zielgruppe verstehen können.

![Der Abschnitt „Identitäten“ im Arbeitsbereich einer einzelnen Zielgruppe.](/help/assets/setup/add-manage-audiences/audience-details-identities.png){zoomable="yes"}

Wenn Sie den Mauszeiger über die einzelnen Abschnitte der Aufschlüsselung der Übereinstimmungsschlüssel bewegen, erhalten Sie eine genaue Identitätsanzahl für den entsprechenden Schlüssel.

![Der Abschnitt „Identitäten“ im Arbeitsbereich einer einzelnen Zielgruppe mit einer Aufschlüsselung des Übereinstimmungsschlüssels wird angezeigt.](/help/assets/setup/add-manage-audiences/audience-details-identities.png)

#### Kategorien {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="Kategorien"
>abstract="Zielgruppen können mit Tags versehen werden, um sie einfach zu organisieren, zu filtern und abzurufen. Eine Zielgruppe kann mit Tags mehrerer Kategorien versehen werden und diese Kategorie-Tags können anschließend verwendet werden, um die gewünschten Zielgruppen in anderen Bereichen des Produkts zu filtern."

Um die Organisation, Filterung und den Abruf von Audiences zu vereinfachen, können Sie Ihre Audiences mit Tags versehen. Sie können eine Zielgruppe mit mehreren Kategorien taggen. Anschließend können Sie diese Kategorietags verwenden, um Ihre gewünschten Zielgruppen im Produktbereich [Entdecken](/help/guide/collaborate/discover.md) zu filtern, wenn Sie Berichte zur Zielgruppenüberschneidung ausführen.

Um Kategorien hinzuzufügen, wählen Sie die Option **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Kategorien]** aus.

![Der Abschnitt Kategorien im Arbeitsbereich einer einzelnen Zielgruppe.](/help/assets/setup/add-manage-audiences/audience-details-categories.png){zoomable="yes"}

Das **[!UICONTROL Kategorien]** wird angezeigt, in dem Sie die Kategorien auswählen können, die Sie der Audience hinzufügen möchten. Um eine einzelne Kategorie auszuwählen, aktivieren Sie das Kontrollkästchen neben dem Kategorienamen.

![Das Dialogfeld Kategorien mit den verfügbaren Kategorien wird angezeigt.](/help/assets/setup/add-manage-audiences/audience-details-categories-select.png){zoomable="yes"}

#### Zugriff auf Verbindungen {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="Zugriff auf Verbindungen"
>abstract="<p>Zielgruppen können drei Typen aufweisen: öffentlich, privat und benutzerdefiniert.</p><p> Ihre Verfügbarkeit für die Verwendung in Projekten mit Mitwirkenden unterscheidet sich je nach Einstellung für den Verbindungszugriff.</p>"

Die Verfügbarkeit einer Zielgruppe zur Verwendung in Projekten mit Partnern unterscheidet sich je nach Verbindungszugriffseinstellung. Im Abschnitt **[!UICONTROL Verbindungszugriff]** können Sie auswählen, ob die Zielgruppe privat, öffentlich oder nur für bestimmte Verbindungen verfügbar sein soll. Öffentliche Zielgruppen sind in Verbindungen verwendbar und auffindbar.

Um den Verbindungszugriff der Zielgruppe zu aktualisieren, wählen Sie die Option **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Verbindungszugriff]** aus.

![Der Abschnitt „Verbindungszugriff“ des Arbeitsbereichs einer einzelnen Zielgruppe.](/help/assets/setup/add-manage-audiences/audience-details-connection-access.png){zoomable="yes"}

Das **[!UICONTROL Verbindungszugriff]** wird mit drei verfügbaren Verbindungszugriffsoptionen angezeigt:

* **[!UICONTROL Private]**. Diese Zielgruppen stehen *nicht* zur Verwendung in Überschneidungsberichten oder zur Aktivierung in Verbindungen mit Partnern zur Verfügung. Obwohl die Zielgruppen von Kollaborateuren nicht angezeigt oder verwendet werden können, trägt die Population der Zielgruppen weiterhin zur Gesamtpopulation in der Ansicht **[!UICONTROL Alle Zielgruppen]** im Abschnitt [Vergleichen von Zielgruppen](/help/guide/collaborate/discover.md#compare-audiences) bei. Ändern Sie die Einstellung in Öffentlich oder Benutzerdefiniert , um die Zielgruppen in Verbindungen mit Partnern zu verwenden.
* **[!UICONTROL Öffentliche]**. Diese Zielgruppen stehen für die Verwendung in Überschneidungsberichten und für die Aktivierung in Verbindungen mit beliebigen Partnern zur Verfügung.
* **[!UICONTROL Benutzerdefinierte Zielgruppe]**. Diese Zielgruppen sind nur für die Verwendung in Überschneidungsberichten und für die Aktivierung in bestimmten Verbindungen verfügbar. Obwohl die Zielgruppen von Kollaborateuren nicht angezeigt oder verwendet werden können, trägt die Population der Zielgruppen weiterhin zur Gesamtpopulation in der Ansicht **[!UICONTROL Alle Zielgruppen]** im Abschnitt [Vergleichen von Zielgruppen](/help/guide/collaborate/discover.md#compare-audiences) bei.

Wählen Sie die gewünschte Verbindungszugriffsoption aus und klicken Sie dann auf **[!UICONTROL Speichern]**, um die Änderungen anzuwenden.

![Das Dialogfeld „Verbindungszugriff“ mit den verfügbaren Optionen wird angezeigt.](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png){zoomable="yes"}

>[!IMPORTANT]
>
>Unabhängig vom Zugriffsstatus (öffentlich, privat oder benutzerdefiniert) trägt die Population einer beliebigen Zielgruppe zur Population **[!UICONTROL Alle Zielgruppen]** im Abschnitt **[!UICONTROL Zielgruppen vergleichen]** innerhalb eines Projekts bei.

Die Zielgruppenverfügbarkeit für die Verwendung in Projekten mit Partnern unterscheidet sich je nach Verbindungszugriffseinstellung.

#### Sichtbarkeit von Metadaten {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="Sichtbarkeit von Metadaten"
>abstract="<p>Gibt an, welche der Metadaten einer Zielgruppe für andere Mitwirkende sichtbar sind, bevor diese eine Verbindung zu Ihnen oder in Projektansichten herstellen.</p> <p> Die **Anzahl der Identitäten** steuert, ob Ihre Mitwirkende bzw. Ihr Mitwirkender Identitätsanzahlen für Ihre Zielgruppen anzeigen kann, wenn Überschneidungsberichte auf der Registerkarte „Entdeckung“ angezeigt werden. </p><p> Die **Zielgruppenüberschneidung in %** steuert, ob Mitwirkende Überschneidungsprozentsätze zwischen ihren Zielgruppen und Ihren Zielgruppen ermitteln können.</p><p> **[!UICONTROL Zielgruppenindex]** steuert, ob Mitwirkende den Zielgruppenindex in einem Projekt anzeigen können. Diese Funktion ist nur verfügbar, wenn mindestens drei aktive Zielgruppen vorhanden sind.</p> <br> Damit die Einstellungen für die Metadatensichtbarkeit wirksam werden, muss die Zielgruppe auf „Öffentlich“ oder „Benutzerdefiniert“ festgelegt sein."

>[!NOTE]
>
>Wenn für Ihren Mitarbeiter alle Zielgruppen auf „privat“ festgelegt sind, ist der Abschnitt **[!UICONTROL Relevante Zielgruppen]** im Arbeitsbereich **[!UICONTROL Entdecken]** leer. Weitere Informationen finden Sie im Handbuch [Entdecken](/help/guide/collaborate/discover.md#relevant-audiences).

Die Sichtbarkeit von Metadaten gibt die Sichtbarkeit der Metadaten einer Zielgruppe für andere Mitwirkende an, bevor diese eine Verbindung mit Ihnen herstellen oder in verschiedenen Projektansichten. Um die Metadatensichtbarkeit der Zielgruppe zu aktualisieren, wählen Sie die Option **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Metadatensichtbarkeit]** aus.

![Der Abschnitt „Metadaten-Sichtbarkeit“ des Arbeitsbereichs einer einzelnen Zielgruppe.](/help/assets/setup/add-manage-audiences/audience-details-metadata-visibility.png){zoomable="yes"}

Das **[!UICONTROL Metadaten-Sichtbarkeit]** wird angezeigt, in dem Sie die Sichtbarkeitseinstellungen für die Zielgruppe konfigurieren können. Es gibt zwei Einstellungen für die Sichtbarkeit von Metadaten, die Sie für jede Zielgruppe konfigurieren können:

**[!UICONTROL Anzahl der Identitäten anzeigen]** Mit dieser Einstellung steuern Sie, ob Ihr Mitarbeiter beim Anzeigen von Überschneidungsberichten auf der Registerkarte &quot;[&quot; innerhalb ](/help/guide/collaborate/discover.md#discover-overlaps) Projekts Identitätszahlen für Ihre Zielgruppen anzeigen kann.

**[!UICONTROL Zielgruppenüberschneidung anzeigen %]**: Diese Einstellung steuert, ob Mitwirkende in der Lage sind, [Überschneidungsprozentsätze zu ermitteln](/help/guide/collaborate/discover.md#compare-audiences) zwischen ihren Zielgruppen und Ihren Zielgruppen.

**[!UICONTROL Zielgruppenindex]**: Bei Festlegung auf „true“ können Ihre Mitarbeiter den [Zielgruppenindex](/help/guide/collaborate/discover.md#audience-index-score) innerhalb eines Projekts anzeigen. Diese Funktion ist nur verfügbar, wenn mindestens drei aktive Zielgruppen vorhanden sind.

>[!NOTE]
>
>Damit die Einstellungen für die Metadatensichtbarkeit wirksam werden, muss die Zielgruppe auf „Öffentlich“ oder „Benutzerdefiniert“ eingestellt sein.

![Das Dialogfeld „Metadatensichtbarkeit“ mit den verfügbaren Optionen wird angezeigt.](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png){zoomable="yes"}

## Mehrere Zielgruppen bearbeiten {#edit-audiences}

Im Zielgruppen-Dashboard können Sie mehrere Zielgruppen gleichzeitig bearbeiten. Wählen Sie dazu die Zielgruppen aus, die Sie bearbeiten möchten, indem Sie die Kästchen neben ihren Namen auswählen. Nach Auswahl der Zielgruppen können Sie Aktionen mit den Optionen im Menü „Bearbeiten“ durchführen.

![Der Arbeitsbereich „Meine Zielgruppen“ mit zwei ausgewählten Zielgruppen und dem hervorgehobenen Menü „Bearbeiten“.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit.png)

### Sichtbarkeit von Massenbearbeitungs-Metadaten {#bulk-edit-metadata-visibility}

Wenn Ihre Zielgruppen im Zielgruppen-Dashboard ausgewählt sind, wählen Sie **[!UICONTROL Metadaten-Sichtbarkeit bearbeiten]** aus dem Menü „Bearbeiten“ aus.

![Der Arbeitsbereich „Meine Zielgruppen“ mit hervorgehobener Option „Metadaten-Sichtbarkeit bearbeiten“.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-metadata.png)

Das **[!UICONTROL Metadaten-Sichtbarkeit]** wird angezeigt, in dem Sie die Sichtbarkeitseinstellungen für die ausgewählten Zielgruppen konfigurieren können. Standardmäßig ist keine der Optionen ausgewählt. Wählen Sie die Optionen aus, die Sie auf alle ausgewählten Zielgruppen anwenden möchten, und wählen Sie dann **[!UICONTROL Speichern]**.

![Das Dialogfeld „Metadatensichtbarkeit“ mit den verfügbaren Optionen wird angezeigt.](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png)

### Massenbearbeitung des Verbindungszugriffs {#bulk-edit-connection-access}

Wenn Ihre Zielgruppen im Zielgruppen-Dashboard ausgewählt sind, wählen Sie **[!UICONTROL Verbindungszugriff bearbeiten]** aus dem Menü „Bearbeiten“ aus.

![Der Arbeitsbereich „Meine Zielgruppen“ mit hervorgehobener Option „Verbindungszugriff bearbeiten“.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-connection-access.png)

Das **[!UICONTROL Verbindungszugriff]** wird angezeigt, in dem Sie die Zugriffseinstellungen für die ausgewählten Zielgruppen konfigurieren können. Standardmäßig ist die Option **[!UICONTROL Private Zielgruppe]** ausgewählt. Wählen Sie die Optionen aus, die Sie auf alle ausgewählten Zielgruppen anwenden möchten, und wählen Sie dann **[!UICONTROL Speichern]**.

![Das Dialogfeld „Verbindungszugriff“ mit den verfügbaren Optionen wird angezeigt.](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png)

### Massenbearbeitung von Zielgruppennamen und -beschreibungen {#bulk-edit-audience-names-descriptions}

Wenn Ihre Zielgruppen im Zielgruppen-Dashboard ausgewählt sind, wählen Sie **[!UICONTROL Name und Beschreibung bearbeiten]** aus dem Menü „Bearbeiten“.

![Der Arbeitsbereich „Meine Zielgruppen“ mit hervorgehobener Option „Namen und Beschreibung bearbeiten“.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-name-description.png)

Das **[!UICONTROL Name und Beschreibung]** wird angezeigt, in dem Sie den Namen und die Beschreibung für jede ausgewählte Zielgruppe konfigurieren können. Standardmäßig werden die aktuellen Namen und Beschreibungen für jede Zielgruppe angezeigt. Nehmen Sie die gewünschten Änderungen vor und klicken Sie auf **[!UICONTROL Speichern]**.

![Das Dialogfeld „Name und Beschreibung“ mit den verfügbaren Optionen wird angezeigt.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-name-description-dialog.png)

### Massenbearbeitung von Kategorien {#bulk-edit-categories}

Wenn Ihre Zielgruppen im Zielgruppen-Dashboard ausgewählt sind, wählen Sie **[!UICONTROL Kategorien bearbeiten]** aus dem Menü „Bearbeiten“.

![Der Arbeitsbereich „Meine Zielgruppen“ mit hervorgehobener Option „Kategorien bearbeiten“.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-categories.png)

Das **[!UICONTROL Kategorien]** wird angezeigt, in dem Sie die Kategorien für jede ausgewählte Zielgruppe konfigurieren können. Standardmäßig werden keine Kategorien ausgewählt. Um eine Kategorie auszuwählen, wählen Sie zunächst die Hauptkategorie und dann die Unterkategorien aus, die Sie einbeziehen möchten. Nehmen Sie die gewünschten Änderungen vor und klicken Sie auf **[!UICONTROL Speichern]**.

![Das Dialogfeld Kategorien mit den verfügbaren Optionen wird angezeigt.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-categories-dialog.png)

## Nächste Schritte

Nach der Beschaffung von Zielgruppen ist es an der Zeit, Mitarbeiter zu finden, mit denen [verbinden](/help/guide/connect/establishing-connections.md) um an Projekten zusammenzuarbeiten.
