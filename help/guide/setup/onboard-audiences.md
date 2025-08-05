---
title: Source und Verwalten von Audiences
description: Erfahren Sie, wie Sie Zielgruppen in Adobe Real-Time CDP Collaboration beschaffen und verwalten.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: 608706d00124372ac59209478ab551a3a6ce0226
workflow-type: tm+mt
source-wordcount: '2897'
ht-degree: 18%

---

# Source und Verwalten von Audiences

{{limited-availability-release-note}}

Zielgruppen sind spezifische Benutzergruppen oder Kundinnen bzw. Kunden, die anhand verschiedener Attribute segmentiert werden. Diese ermöglichen es den Mitarbeitern, bei zielgerichteten Marketing- und personalisierten Erlebnissen zusammenzuarbeiten, um effektivere Werbekampagnen zu ermöglichen. In diesem Handbuch wird beschrieben, wie Sie Zielgruppen in Real-Time CDP Collaboration beschaffen, das Zielgruppen-Dashboard anzeigen und einzelne Zielgruppen verwalten.

>[!BEGINSHADEBOX]

Was Sie auf dieser Dokumentationsseite finden:

* [Source-Zielgruppen in Collaboration](#source-audiences)
* [Anzeigen des Dashboards „Zielgruppen“](#view-audiences-dashboard)
* [Anzeigen einzelner Zielgruppen](#view-individual-audiences)

>[!ENDSHADEBOX]

## Source-Zielgruppen in Collaboration {#source-audiences}

>[!IMPORTANT]
>
>Um Zielgruppen beziehen zu können, muss den Benutzenden eine Rolle zugewiesen werden, die zwei Profilverwaltungsberechtigungen enthält: **[!UICONTROL Profile anzeigen]** und **[!UICONTROL Segmente]**. Informationen zum Zuweisen der erforderlichen Berechtigungen finden Sie im Handbuch [Zielgruppen-Beschaffung](../permissions/overview.md#audience-sourcing) unter Berechtigungen.

Bevor Sie Zielgruppen mit Partnern aktivieren und Überschneidungsberechnungen durchführen können, müssen die Zielgruppen in Collaboration bezogen werden. Um Zielgruppen zu beziehen, befolgen Sie die Workflow-Schritte im folgenden Abschnitt.

Wählen Sie im Arbeitsbereich **[!UICONTROL Setup]** **[!UICONTROL auf der Registerkarte „Meine Zielgruppen]** das Symbol zum Hinzufügen (![Hinzufügen) aus.](/help/assets/icons/plus.png)) und wählen Sie dann **[!UICONTROL Audience]** aus. Wenn dies Ihre erste Zielgruppe ist, können Sie auch die Option **[!UICONTROL Hinzufügen] auswählen**.

![Mein Zielgruppen-Arbeitsbereich mit hervorgehobener Option „Hinzufügen“ und hervorgehobener Option „Zielgruppen“.](/help/assets/setup/add-manage-audiences/add-audiences.png)

### Auswählen der Datenverbindung {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="Marketing-Aktionen"
>abstract="<p>Verwenden Sie Marketing-Aktionen, um zu steuern, welche Zielgruppendaten aus Experience Platform in Real-Time CDP Collaboration importiert werden sollen. Die Marketing-Aktion <strong>Data Collaboration</strong> unterstützt Datennutzungs-Labels vom Typ C4, C5 und C9. Die Marketing-Aktion <strong>Datenwissenschaft</strong> unterstützt das Datennutzungs-Label vom Typ C9.</p> <p> <ul><li> Wenn das Kontrollkästchen <em>aktiviert</em> ist, werden alle mit den oben genannten Labels in Experience Platform markierten Daten, ausgeschlossen und <strong>nicht</strong> in Real-Time CDP Collaboration übertragen.</li><li> Wenn das Kontrollkästchen <em>deaktiviert</em> ist, gibt es keine Einschränkung für Daten aus Experience Platform, die in Real-Time CDP Collaboration importiert werden können.</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=de" text="Datennutzungs-Labels – Übersicht"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html?lang=de" text="Glossar der Datennutzungs-Labels"

>[!IMPORTANT]
>
>Nachdem Sie Ihre erste Datenverbindung hergestellt und Ihre erste Zielgruppe importiert haben, können Sie mehrere Zielgruppen aus der vorhandenen Datenverbindung importieren. Beim Hinzufügen zusätzlicher Zielgruppen beginnen Sie mit dem Schritt [Zielgruppe auswählen](#select-audiences), da die Datenverbindung bereits hergestellt wurde.

Eine Datenverbindung ist die Datenquelle, aus der Sie Zielgruppen beziehen. Derzeit wird nur Adobe Experience Platform als Datenverbindung unterstützt.

Alle Einstellungen wie die Planung, die Sie für Ihre Datenverbindung konfigurieren, werden auf alle Zielgruppen angewendet, die von dieser Datenverbindung bezogen werden.

>[!TIP]
>
>Es gibt einen separaten Workflow, in dem Sie Ihre Datenverbindungen anzeigen und bearbeiten können. Weitere Informationen finden Sie im [Verwalten von Datenverbindungen](/help/guide/setup/manage-data-connection.md).

Um mit dem Hinzufügen Ihrer Datenverbindung zu beginnen, wählen Sie **[!UICONTROL Neue Datenverbindung hinzufügen]** und dann **[!UICONTROL Weiter]** aus.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit hervorgehobener Option „Neue Datenverbindung hinzufügen“.](/help/assets/setup/add-manage-audiences/add-data-connection.png)

#### Datenquelle auswählen

Als Nächstes wählen Sie die Quelle für Ihre Datenverbindung. Zu den verfügbaren Quellen gehören:

* **Adobe Experience Platform**: Wählen Sie diese Option, um Ihre Zielgruppen aus Adobe Experience Platform einzubringen.
* **CSV-Datei** (künftige Version): Laden Sie eine CSV-Datei hoch, die Ihre Zielgruppendaten enthält, um Daten schnell und einfach aufzunehmen.
* **Amazon Web Services** (zukünftige Version): Stellen Sie eine Verbindung zu Ihrem Amazon S3-Speicher her, um Zielgruppendaten direkt aus Ihren S3-Buckets zu beziehen.
* **Snowflake** (zukünftige Version): Verwenden Sie Ihr Snowflake Data Warehouse, um Zielgruppendaten nahtlos abzurufen.
* **Google Cloud Platform** (zukünftige Version): Stellen Sie eine Verbindung zu Ihrem Google Cloud-Speicher her, um Zielgruppendaten direkt aus Ihren GCS-Buckets zu beziehen.

Wählen Sie Ihre Datenquelle und dann **[!UICONTROL Weiter]** aus.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit hervorgehobener Option &quot;Adobe Experience Platform&quot;.](/help/assets/setup/add-manage-audiences/select-data-connection-source.png)

#### Sandbox auswählen

Nach Auswahl der Datenquelle müssen Sie die Sandbox auswählen, die die Zielgruppen enthält, die Sie für Collaboration verwenden möchten. Wählen Sie die Sandbox aus der Liste der verfügbaren Sandboxes aus und klicken Sie dann auf **[!UICONTROL Weiter]**

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit ausgewählter Sandbox.](/help/assets/setup/add-manage-audiences/select-sandbox.png)

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

![Der Arbeitsbereich „Zielgruppen hinzufügen“ im Abschnitt „Governance-Richtlinie und Durchsetzungsaktionen“.](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png)

Nachdem Sie die Marketing-Aktionen und Einverständnisregeln ausgewählt haben, klicken Sie auf **[!UICONTROL Weiter]**, um mit dem nächsten Schritt fortzufahren. Es erscheint ein Bestätigungsdialogfeld, in dem Sie aufgefordert werden, die Bedingungen zu akzeptieren. Aktivieren Sie das Kontrollkästchen und klicken Sie dann zur Bestätigung **[!UICONTROL OK]**.

![Das Dialogfeld „Governance-Richtlinie“ und „Durchsetzungsaktionen“ mit hervorgehobenem Kontrollkästchen und hervorgehobener Option „OK“.](/help/assets/setup/add-manage-audiences/data-collaboration-consent-confirmation.png)

### Details angeben

Geben Sie als Nächstes einen Namen und eine Beschreibung für Ihre Datenverbindung an. Diese Informationen helfen Ihnen später bei der Identifizierung der Datenverbindung.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit der Option, einen Namen und eine Beschreibung anzugeben.](/help/assets/setup/add-manage-audiences/data-connection-details.png)

### Zuordnen von Feldern {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="Quellfelder"
>abstract="Quellfelder sind Identity-Namespaces und Attribute aus Ihrer Implementierung von Experience Platform. Sie können diese Zielfeldern zuordnen, die in Collaboration definiert sind."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="Zielfelder"
>abstract="Derzeit sind Hash-E-Mails die einzigen unterstützten Übereinstimmungsschlüssel."

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

Als Nächstes wählen Sie Quellfelder aus, die Zielfeldern in Collaboration zugeordnet werden sollen.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit der Option, Quellfelder Zielfeldern zuzuordnen.](/help/assets/setup/add-manage-audiences/add-map-fields.png)

>[!TIP]
>
>Sie können demselben Zielfeld mehrere Quellfelder zuordnen. Wenn sich beispielsweise E-Mail-Adressen in zwei separaten Feldern in Experience Platform befinden, können Sie diese jeweils dem Zielfeld **[!UICONTROL gehashte E-Mail]** als zwei separate Zeilen zuordnen.

>[!BEGINSHADEBOX]

**[!UICONTROL Source-Felder]** sind Identitäts-Namespaces und -Attribute aus Experience Platform. So existieren die Identitäten in der Plattform, von der Sie Daten beziehen. Source-Felder werden den in Collaboration definierten Zielfeldern zugeordnet.

**[!UICONTROL Zielfelder]** geben an, wie die Identitäten in Collaboration referenziert werden. Derzeit sind Hash-E-Mails die einzigen unterstützten Übereinstimmungsschlüssel.

Verwenden Sie die **[!UICONTROL Umwandlung anwenden]**, wenn Sie (*gehashte)* aus Ihrer Quelle importieren. In diesem Fall wendet Collaboration den Hash-Wert an und wandelt die Felder um. Der von Adobe verwendete Hash-Algorithmus ist SHA256.

>[!ENDSHADEBOX]

Wählen Sie das leere Quellfeld neben dem Zielfeld aus. Das **[!UICONTROL Quellfeld auswählen]** wird angezeigt. Wählen Sie zwischen den **[!UICONTROL Identity-]**) und **[!UICONTROL Profilattribute]**, um das gewünschte Quellfeld zu finden, und wählen Sie dann das Feld aus der Liste aus. Sie können auch die Suchoption verwenden, um das gewünschte Feld zu finden.

![Das Dialogfeld „Quellfeld auswählen“ mit den angezeigten E-Mail-Optionen.](/help/assets/setup/add-manage-audiences/select-source-field.png)

Um mehrere E-Mail-Felder zu verarbeiten, ordnen Sie das nicht gehashte E-Mail-Quellfeld mithilfe von **[!UICONTROL Umwandlung anwenden]** zu.

![Der Arbeitsbereich Zielgruppen hinzufügen mit den E-Mail-Quellfeldern, die dem Zielfeld zugeordnet sind, wobei Umwandlung anwenden für ein Feld aktiviert ist.](/help/assets/setup/add-manage-audiences/apply-transformation.png)

Fahren Sie mit dem Hinzufügen von Zuordnungspaaren fort und klicken Sie auf **[!UICONTROL Weiter]**.

### Zeitplan {#schedule}

Als Nächstes planen Sie, wann die Zielgruppen gefüllt werden sollen. Die Zielgruppe wird gemäß diesem Zeitplan aktualisiert.

![Der Arbeitsbereich „Zielgruppe hinzufügen“ mit den angezeigten Planungsoptionen.](/help/assets/setup/add-manage-audiences/audience-scheduling.png)

>[!IMPORTANT]
>
>Durch die Anpassung der Aktualisierungshäufigkeit der Zielgruppe können Sie die [Audience-Management-](/help/guide/setup/my-activity.md#types-of-activities)&quot; verwalten, die pro Zielgruppenaktualisierung berechnet wird. Die Auswahl einer höheren Häufigkeit kann sich auf die Aktualität der Daten auswirken, die für Zielgruppen-Discover-Berichte und die Zielgruppen-Aktivierung verfügbar sind.

Wählen Sie aus der Dropdown-Liste „Häufigkeit“ die Häufigkeit **[!UICONTROL Aktualisierung]** Zielgruppe aus.

![Der Arbeitsbereich Zielgruppen-Planung hinzufügen mit geöffnetem Dropdown-Menü „Häufigkeit“.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png)

Wählen Sie anschließend den **[!UICONTROL Datumsbereich]** aus. Das Startdatum ist das Datum, an dem die Zielgruppe mit Profilen befüllt wird. Das Enddatum ist, an dem die Aktualisierung der Zielgruppe beendet wird.

![Die Option Zielgruppen hinzufügen im Planungsarbeitsbereich mit Datumsbereich wird angezeigt.](/help/assets/setup/add-manage-audiences/audience-scheduling-date-range.png)

>[!IMPORTANT]
>
>Nach dem Enddatum im Datumsbereich werden alle Zielgruppen, die von dieser Datenverbindung bezogen werden, nicht mehr aktualisiert. Um die Verbindung zu erneuern, folgen Sie der Anleitung [Datenverbindung verwalten](/help/guide/setup/manage-data-connection.md).

### Zielgruppen auswählen {#select-audiences}

Nach Auswahl der Zielgruppenquelle wählen Sie bestimmte Zielgruppen aus, die einbezogen werden sollen. Verwenden Sie die Such- und Filteroptionen, um die relevanten Zielgruppen aus Ihrer Datenquelle zu finden. Wählen Sie die gewünschten Zielgruppen aus und klicken Sie dann auf **[!UICONTROL Weiter]**.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit einer Liste verfügbarer Zielgruppen.](/help/assets/setup/add-manage-audiences/select-audience.png)

### Überprüfung

Überprüfen Sie alle Konfigurationen und Einstellungen, bevor Sie das Hinzufügen der Zielgruppe abschließen. Stellen Sie sicher, dass alle Details korrekt sind, und wählen Sie **[!UICONTROL Abschließen]** aus, um die Erstellung Ihrer Datenverbindung abzuschließen.

![Der Arbeitsbereich „Zielgruppen hinzufügen“ mit allen ausgewählten Konfigurationen wird angezeigt.](/help/assets/setup/add-manage-audiences/review-connection.png)

## Anzeigen des Dashboards „Zielgruppen“ {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="Fehlende Identitäten"
>abstract="Die Anzahl der Identitäten ist nach der nächsten Aktualisierung der Datenverbindung gemäß dem konfigurierten Zeitplan verfügbar. Die erste Aktualisierung erfolgt normalerweise innerhalb von 24 Stunden nach der Einrichtung der Datenverbindung. Laufende Aktualisierungen folgen dem konfigurierten Zeitplan."

Nach der Beschaffung von Zielgruppen zeigt der **[!UICONTROL Meine Zielgruppen]** Arbeitsbereich alle Zielgruppen an, die derzeit in Collaboration bezogen werden.

Jede Zielgruppe enthält einen Überblick über die folgenden Informationen:

| Element | Beschreibung |
|----------|---------|
| **[!UICONTROL Identitäten]** | Gibt die Anzahl der in dieser Zielgruppe vorhandenen Identitäten an. Beachten Sie Folgendes: Wenn dasselbe Profil zwei oder mehr Identitäten hat und diese Identitäten als Übereinstimmungsschlüssel im Projekt verwendet werden, wird das Profil zweimal in der Zählung angezeigt. |
| **[!UICONTROL Status]** | Gibt an, ob die Zielgruppe aktiv ist und in Projekten verwendet werden kann. Der Status **[!UICONTROL Ausstehend]** gibt an, dass die Zielgruppe gerade erst abgerufen wurde und Identitäten noch ausgefüllt werden müssen. Die Zielgruppen der Quelle werden nach der ersten Aktualisierung, die in der Regel innerhalb von 24 Stunden nach der Einrichtung der Datenverbindung erfolgt, mit Profilen gefüllt. |
| **[!UICONTROL Quelle]** | Gibt an, woher die Zielgruppe stammt. In der aktuellen Version von Collaboration ist Experience Platform die einzige unterstützte Quelle. |
| **[!UICONTROL Datenverbindung]** | Die Datenverbindung, von der die Zielgruppe stammt. Sie können den Namen auswählen, um die Datenverbindung anzuzeigen. |
| **[!UICONTROL Verbindungszugriff]** | Definiert, ob die Zielgruppe privat oder öffentlich ist. Öffentliche Zielgruppen sind in Überschneidungsberichten auffindbar und können innerhalb eines Projekts aktiviert werden. |
| **[!UICONTROL Erstellt]** | Gibt an, wann die Zielgruppe ursprünglich in Collaboration aufgenommen wurde. |
| **[!UICONTROL Zuletzt aktualisiert]** | Gibt das letzte Datum und die letzte Uhrzeit der Aktualisierung der Zielgruppe in Collaboration an. Dies bezieht sich nicht auf den Zeitpunkt der letzten Aktualisierung der Zielgruppe, sondern auf den Zeitpunkt der letzten Änderung der Konfiguration oder der Metadaten der Zielgruppe. |

![Der Arbeitsbereich Meine Zielgruppe mit allen aus der Quelle stammenden Zielgruppen.](/help/assets/setup/add-manage-audiences/audiences-workspace.png)

Um Schnellaktionen für eine Zielgruppe durchzuführen, klicken Sie auf die **mit den Auslassungspunkten…** neben dem Namen der Zielgruppe. Die folgenden Optionen sind verfügbar:

* **[!UICONTROL Kategorien bearbeiten]** ermöglicht das Hinzufügen verschiedener Kategorie-Tags zur Audience. Weitere Informationen finden Sie im Abschnitt [Kategorien](#categories) unten.
* **[!UICONTROL Löschen]** wird die Zielgruppe aus der Datenverbindung gelöscht.

![Der Arbeitsbereich „Meine Zielgruppen“ mit geöffnetem Menü und hervorgehobenen Optionen „Kategorien bearbeiten“ und „Löschen“.](/help/assets/setup/add-manage-audiences/audiences-ellipsis-menu.png)

## Anzeigen einzelner Zielgruppen {#view-individual-audiences}

Um weitere Informationen anzuzeigen und Konfigurationen für eine einzelne Zielgruppe zu bearbeiten, wählen Sie die Zielgruppe im Arbeitsbereich **[!UICONTROL Meine Zielgruppen]** aus. Der Zielgruppen-Arbeitsbereich zeigt detaillierte Informationen zur ausgewählten Zielgruppe an, einschließlich Details, Identitäten, Kategorien, Verbindungszugriff und Einstellungen für die Sichtbarkeit von Metadaten.

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

![Arbeitsbereich einer einzelnen Zielgruppe.](/help/assets/setup/add-manage-audiences/audience-details.png)

Darüber hinaus sind die folgenden Steuerelemente im Zielgruppen-Arbeitsbereich verfügbar:

* **[!UICONTROL Löschen]**: Entfernen Sie die Zielgruppe aus Ihrer Datenverbindung.
* **[!UICONTROL Bearbeiten]**: Name oder Beschreibung der Zielgruppe bearbeiten.

![Der Arbeitsbereich einer einzelnen Zielgruppe mit hervorgehobener Option „Bearbeiten“ und „Löschen“.](/help/assets/setup/add-manage-audiences/audience-details-edit-delete.png)

Als Nächstes können Sie die folgenden Abschnitte im Arbeitsbereich der Zielgruppe aktualisieren:

* [Identitäten](#identities)
* [Kategorien](#categories)
* [Zugriff auf Verbindungen](#connection-access)
* [Sichtbarkeit von Metadaten](#metadata-visibility)

### Identitäten {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="Identitäten"
>abstract="Eine Aufschlüsselungsansicht der Identitäten, aus denen diese Zielgruppe besteht, sowie eine Gesamtanzahl der Profile mit den entsprechenden Identitäten."

Im Abschnitt **[!UICONTROL Identitäten]** wird die Anzahl der Profile angegeben, die in der Zielgruppe mit einer der Identitäten vorhanden sind, die Sie beim Beschaffen der Zielgruppe ausgewählt haben. Der Abschnitt enthält auch eine Aufschlüsselung der Identität, sodass Sie feststellen können, welche Identitäten den größten Teil der Zielgruppen-Population ausmachen.

![Der Abschnitt „Identitäten“ im Arbeitsbereich einer einzelnen Zielgruppe.](/help/assets/setup/add-manage-audiences/audience-details-identities.png)

### Kategorien {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="Kategorien"
>abstract="Zielgruppen können mit Tags versehen werden, um sie einfach zu organisieren, zu filtern und abzurufen. Eine Zielgruppe kann mit Tags mehrerer Kategorien versehen werden und diese Kategorie-Tags können anschließend verwendet werden, um die gewünschten Zielgruppen in anderen Bereichen des Produkts zu filtern."

Um die Organisation, Filterung und den Abruf von Audiences zu vereinfachen, können Sie Ihre Audiences mit Tags versehen. Sie können eine Zielgruppe mit mehreren Kategorien taggen. Anschließend können Sie diese Kategorietags verwenden, um Ihre gewünschten Zielgruppen im Produktbereich [Entdecken](/help/guide/collaborate/discover.md) zu filtern, wenn Sie Berichte zur Zielgruppenüberschneidung ausführen.

Um Kategorien hinzuzufügen, wählen Sie die Option **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Kategorien]** aus.

![Der Abschnitt Kategorien im Arbeitsbereich einer einzelnen Zielgruppe.](/help/assets/setup/add-manage-audiences/audience-details-categories.png)

Das **[!UICONTROL Kategorien]** wird angezeigt, in dem Sie die Kategorien auswählen können, die Sie der Audience hinzufügen möchten. Um eine einzelne Kategorie auszuwählen, aktivieren Sie das Kontrollkästchen neben dem Kategorienamen.

![Das Dialogfeld Kategorien mit den verfügbaren Kategorien wird angezeigt.](/help/assets/setup/add-manage-audiences/audience-details-categories-select.png)

### Zugriff auf Verbindungen {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="Zugriff auf Verbindungen"
>abstract="<p>Zielgruppen können drei Typen aufweisen: öffentlich, privat und benutzerdefiniert.</p><p> Ihre Verfügbarkeit für die Verwendung in Projekten mit Mitwirkenden unterscheidet sich je nach Einstellung für den Verbindungszugriff. Die Zugriffsberechtigung für die Verbindung kann immer von der privaten in die öffentliche geändert werden. Diese Einstellung kann jedoch nicht geändert werden, sobald eine Zielgruppe mit Partnern aktiviert wurde.</p>"

Die Verfügbarkeit einer Zielgruppe zur Verwendung in Projekten mit Partnern unterscheidet sich je nach Verbindungszugriffseinstellung. Im Abschnitt **[!UICONTROL Verbindungszugriff]** können Sie auswählen, ob die Zielgruppe privat oder öffentlich sein soll. Öffentliche Zielgruppen sind in Verbindungen verwendbar und auffindbar.

Um den Verbindungszugriff der Zielgruppe zu aktualisieren, wählen Sie die Option **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Verbindungszugriff]** aus.

![Der Abschnitt „Verbindungszugriff“ des Arbeitsbereichs einer einzelnen Zielgruppe.](/help/assets/setup/add-manage-audiences/audience-details-connection-access.png)

Das **[!UICONTROL Verbindungszugriff]** wird mit drei verfügbaren Verbindungszugriffsoptionen angezeigt:

* **[!UICONTROL Private]**. Diese Zielgruppen stehen *nicht* zur Verwendung in Überschneidungsberichten oder zur Aktivierung in Verbindungen mit Partnern zur Verfügung. Obwohl die Zielgruppen von Kollaborateuren nicht angezeigt oder verwendet werden können, trägt die Population der Zielgruppen weiterhin zur Gesamtpopulation in der Ansicht **[!UICONTROL Alle Zielgruppen]** im Abschnitt [Vergleichen von Zielgruppen](/help/guide/collaborate/discover.md#compare-audiences) bei. Ändern Sie die Einstellung in Öffentlich oder Benutzerdefiniert , um die Zielgruppen in Verbindungen mit Partnern zu verwenden.
* **[!UICONTROL Öffentliche]**. Diese Zielgruppen stehen für die Verwendung in Überschneidungsberichten und für die Aktivierung in Verbindungen mit beliebigen Partnern zur Verfügung.
* **[!UICONTROL Benutzerdefinierte Zielgruppe]**. Diese Zielgruppen sind nur für die Verwendung in Überschneidungsberichten und für die Aktivierung in bestimmten Verbindungen verfügbar. Obwohl die Zielgruppen von Kollaborateuren nicht angezeigt oder verwendet werden können, trägt die Population der Zielgruppen weiterhin zur Gesamtpopulation in der Ansicht **[!UICONTROL Alle Zielgruppen]** im Abschnitt [Vergleichen von Zielgruppen](/help/guide/collaborate/discover.md#compare-audiences) bei.

Wählen Sie die gewünschte Verbindungszugriffsoption aus und klicken Sie dann auf **[!UICONTROL Speichern]**, um die Änderungen anzuwenden.

![Das Dialogfeld „Verbindungszugriff“ mit den verfügbaren Optionen wird angezeigt.](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png)

>[!IMPORTANT]
>
>Unabhängig vom Zugriffsstatus (öffentlich, privat oder benutzerdefiniert) trägt die Population einer beliebigen Zielgruppe zur Population **[!UICONTROL Alle Zielgruppen]** im Abschnitt **[!UICONTROL Zielgruppen vergleichen]** innerhalb eines Projekts bei.

Die Zielgruppenverfügbarkeit für die Verwendung in Projekten mit Partnern unterscheidet sich je nach Verbindungszugriffseinstellung. Sie können die Zugriffsberechtigung für die Verbindung immer von privat in öffentlich ändern. Sie können diese Einstellung jedoch nicht mehr ändern, sobald eine Zielgruppe aktiviert wurde.

### Sichtbarkeit von Metadaten {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="Sichtbarkeit von Metadaten"
>abstract="<p>Gibt an, welche der Metadaten einer Zielgruppe für andere Mitwirkende sichtbar sind, bevor diese eine Verbindung zu Ihnen oder in Projektansichten herstellen.</p> <p> Die **Anzahl der Identitäten** steuert, ob Ihre Mitwirkende bzw. Ihr Mitwirkender Identitätsanzahlen für Ihre Zielgruppen anzeigen kann, wenn Überschneidungsberichte auf der Registerkarte „Entdeckung“ angezeigt werden. **Zielgruppenüberschneidung %** steuert, ob Mitwirkende Überschneidungsprozentsätze zwischen ihren Zielgruppen und Ihren Zielgruppen ermitteln können."

>[!NOTE]
>
>Wenn für Ihren Mitarbeiter alle Zielgruppen auf „privat“ festgelegt sind, ist der Abschnitt **[!UICONTROL Relevante Zielgruppen]** im Arbeitsbereich **[!UICONTROL Entdecken]** leer. Weitere Informationen finden Sie im Handbuch [Entdecken](/help/guide/collaborate/discover.md#relevant-audiences).

Die Sichtbarkeit von Metadaten gibt die Sichtbarkeit der Metadaten einer Zielgruppe für andere Mitwirkende an, bevor diese eine Verbindung mit Ihnen herstellen oder in verschiedenen Projektansichten. Um die Metadatensichtbarkeit der Zielgruppe zu aktualisieren, wählen Sie die Option **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Metadatensichtbarkeit]** aus.

![Der Abschnitt „Metadaten-Sichtbarkeit“ des Arbeitsbereichs einer einzelnen Zielgruppe.](/help/assets/setup/add-manage-audiences/audience-details-metadata.png)

Das **[!UICONTROL Metadaten-Sichtbarkeit]** wird angezeigt, in dem Sie die Sichtbarkeitseinstellungen für die Zielgruppe konfigurieren können. Es gibt zwei Einstellungen für die Sichtbarkeit von Metadaten, die Sie für jede Zielgruppe konfigurieren können:

**[!UICONTROL Anzahl der Identitäten anzeigen]** Mit dieser Einstellung steuern Sie, ob Ihr Mitarbeiter beim Anzeigen von Überschneidungsberichten auf der Registerkarte &quot;[&quot; innerhalb ](/help/guide/collaborate/discover.md#discover-overlaps) Projekts Identitätszahlen für Ihre Zielgruppen anzeigen kann.

**[!UICONTROL Zielgruppenüberschneidung anzeigen %]**: Diese Einstellung steuert, ob Mitwirkende in der Lage sind, [Überschneidungsprozentsätze zu ermitteln](/help/guide/collaborate/discover.md#compare-audiences) zwischen ihren Zielgruppen und Ihren Zielgruppen.

![Das Dialogfeld „Metadatensichtbarkeit“ mit den verfügbaren Optionen wird angezeigt.](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png)

## Nächste Schritte

Nach der Beschaffung von Zielgruppen ist es an der Zeit, herauszufinden, mit [ Herausgebern ](/help/guide/connect/establishing-connections.md) können, um an Projekten zusammenzuarbeiten.
