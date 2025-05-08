---
title: Importieren und Verwalten von Audiences
description: Erfahren Sie, wie Sie Zielgruppen in Adobe Real-Time CDP Collaboration importieren und verwalten.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: d2ab8e0814d3228e85e03f0e2c1636a6d7167b88
workflow-type: tm+mt
source-wordcount: '2674'
ht-degree: 22%

---

# Importieren und Verwalten von Audiences

{{limited-availability-release-note}}

Zielgruppen sind spezifische Benutzergruppen oder Kundinnen bzw. Kunden, die anhand verschiedener Attribute segmentiert werden. Diese ermöglichen es Werbetreibenden und Publishern, gemeinsam an zielgerichteten Marketing- und personalisierten Erlebnissen zu arbeiten, um effektivere Werbekampagnen zu ermöglichen.

Verwenden Sie diese Seite als Ausgangspunkt, um alle relevanten Metriken zu verstehen, die Sie im Zusammenhang mit Ihren Zielgruppen anzeigen können, sowie die Workflow-Schritte zum Importieren einer Zielgruppe in Adobe Real-Time CDP Collaboration.

>[!TIP]
>
>Verwenden Sie die Informationen auf diesem Bildschirm, um alle erforderlichen Informationen zu Ihren Zielgruppen sowie die [Erkennen und Überschneidungen](/help/guide/collaborate/discover.md) zu erhalten, um einen Einblick zu erhalten, welche Ihrer Zielgruppen für verschiedene Kampagnentypen im Vergleich zum Publisher-Inventar am besten geeignet ist.

>[!BEGINSHADEBOX]

Was Sie auf dieser Dokumentationsseite finden:

* [Importieren von Zielgruppen in Real-Time CDP Collaboration](#import-audiences)
* [Anzeigen des Dashboards „Zielgruppen“](#view-audiences-dashboard)
* [Anzeigen einzelner Zielgruppen](#view-individual-audiences)

>[!ENDSHADEBOX]

## Importieren von Zielgruppen in Real-Time CDP Collaboration {#import-audiences}

>[!IMPORTANT]
>
>Zum Importieren von Audiences muss Ihrem Benutzer eine Rolle zugewiesen werden, die zwei Profilverwaltungsberechtigungen enthält: „Profile anzeigen“ und „Segmente anzeigen“. Informationen zum Zuweisen der erforderlichen Berechtigungen finden Sie im Handbuch [Audience-Import](../permissions/overview.md#audience-importation).

Bevor Sie Zielgruppen für Mitwirkende freigeben und Überschneidungsberechnungen durchführen können, müssen die Zielgruppen in Real-Time CDP Collaboration importiert werden. Gehen Sie zum Importieren von Audiences wie im folgenden Abschnitt beschrieben vor.

![Bildschirm „Meine Zielgruppen“, bevor Zielgruppen zur Organisation hinzugefügt wurden.](/help/assets/setup/add-manage-audiences/org-without-audiences-added.png)

Wählen Sie auf **[!UICONTROL Registerkarte]** Meine Zielgruppen“ das Pluszeichen **+** und anschließend **Zielgruppe** aus.

### Auswählen der Datenverbindung {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="Marketing-Aktionen"
>abstract="<p>Verwenden Sie Marketing-Aktionen, um zu steuern, welche Zielgruppendaten aus Experience Platform in Real-Time CDP Collaboration importiert werden sollen. Die Marketing-Aktion <strong>Data Collaboration</strong> unterstützt Datennutzungs-Labels vom Typ C4, C5 und C9. Die Marketing-Aktion <strong>Datenwissenschaft</strong> unterstützt das Datennutzungs-Label vom Typ C9.</p> <p> <ul><li> Wenn das Kontrollkästchen <em>aktiviert</em> ist, werden alle mit den oben genannten Labels in Experience Platform markierten Daten, ausgeschlossen und <strong>nicht</strong> in Real-Time CDP Collaboration übertragen.</li><li> Wenn das Kontrollkästchen <em>deaktiviert</em> ist, gibt es keine Einschränkung für Daten aus Experience Platform, die in Real-Time CDP Collaboration importiert werden können.</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=de" text="Datennutzungskennzeichnungen – Übersicht"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html?lang=de" text="Glossar der Datennutzungskennzeichnungen"

>[!IMPORTANT]
>
>Nachdem Sie eine Verbindung zu Ihrer ersten Datenverbindung hergestellt und Ihre erste Zielgruppe importiert haben, können Sie mehrere Zielgruppen aus dieser vorhandenen Datenverbindung importieren. In diesem Fall bringt Sie der Workflow direkt zum Schritt [Zielgruppe auswählen](#select-audience), da alle erforderlichen Informationen aus den anderen Schritten aus der vorhandenen Verbindung importiert werden.

Eine Datenverbindung ist die Datenquelle, aus der Sie Zielgruppen in Real-Time CDP Collaboration importieren. Für die erste Version von Real-Time CDP Collaboration wird nur Adobe Experience Platform als Datenverbindung unterstützt.

Alle Einstellungen wie Identitätszuordnung oder Planung, die Sie für Ihre Datenverbindung konfigurieren, werden auf alle Zielgruppen angewendet, die aus dieser Datenverbindung importiert werden.

>[!TIP]
>
>Es gibt einen separaten Workflow, in dem Sie jederzeit alle Datenverbindungen anzeigen und bearbeiten können, die Sie in diesem Schritt hinzugefügt haben. Weitere Informationen [Verwalten von Datenverbindungen](/help/guide/setup/manage-data-connection.md).

![Quellbildschirm der Zielgruppe auswählen mit Optionen für AEP RTCDP, CSV File, Amazon S3 und Snowflake.](/help/assets/setup/add-manage-audiences/Step-Select-Audience-Source.png)

#### Datenquelle auswählen

In diesem Schritt wählen Sie die Quelle Ihrer Zielgruppendaten aus. Zu den verfügbaren Quellen gehören:

* **Adobe Experience Platform**: Wählen Sie diese Option, um Ihre Zielgruppen aus Adobe Experience Platform Real-Time CDP einzubringen.
* **CSV-Datei** (künftige Version): Laden Sie eine CSV-Datei hoch, die Ihre Zielgruppendaten enthält, um Daten schnell und einfach aufzunehmen.
* **Amazon Web Services** (zukünftige Version): Stellen Sie eine Verbindung zu Ihrem Amazon S3-Speicher her, um Zielgruppendaten direkt aus Ihren S3-Buckets zu importieren.
* **Snowflake** (zukünftige Version): Verwenden Sie Ihr Snowflake Data Warehouse, um Zielgruppendaten nahtlos abzurufen.

#### Sandbox auswählen

Nachdem Sie **Adobe Experience Platform** als Datenquelle ausgewählt haben, müssen Sie die Sandbox auswählen, die die Zielgruppen enthält, die Sie importieren möchten.

![Sandbox für den Audience-Import auswählen](/help/assets/setup/add-manage-audiences/import-audiences-select-sandbox.png)

Wählen Sie **[!UICONTROL Weiter]** aus, nachdem Sie die gewünschte Sandbox ausgewählt haben.

#### Governance-Richtlinie und Durchsetzungsmaßnahmen {#governance-policy-and-enforcement-actions}

Als Nächstes müssen Sie sicherstellen, dass für die importierten Daten die richtigen Marketing-Aktionen festgelegt sind. Außerdem müssen Sie für aus Real-Time CDP importierte Daten die Zustimmung zur Verwendung für die Datenerfassung erteilen.

Verwenden Sie Marketing-Aktionen, um zu steuern, welche Zielgruppendaten aus Experience Platform in Real-Time CDP Collaboration importiert werden sollen. Die Marketing-Aktion **Data Collaboration** unterstützt Datennutzungs-Labels vom Typ C4, C5 und C9. Die Marketing-Aktion **Datenwissenschaft** unterstützt das Datennutzungs-Label vom Typ C9.

Lesen Sie mehr über die [C4-, C5- und C9-Datennutzungskennzeichnungen](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}.

* Wenn das Kontrollkästchen *aktiviert* ist, werden alle mit den oben genannten Labels in Experience Platform markierten Daten, ausgeschlossen und *nicht* in Real-Time CDP Collaboration übertragen.
* Wenn das Kontrollkästchen *deaktiviert* ist, gibt es keine Einschränkung für Daten aus Experience Platform, die in Real-Time CDP Collaboration importiert werden können.

Weitere Informationen zu Datennutzungskennzeichnungen finden Sie in der Dokumentation zu Experience Platform:

* [Datennutzungsbezeichnungen – Übersicht](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [Glossar zu Datennutzungskennzeichnungen](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference){target="_blank"}

![Erforderliche Marketing-Aktionen für die Datenerfassung.](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png)

### Details angeben

Geben Sie als Nächstes einen Namen und eine Beschreibung an, damit Sie diese Datenverbindung in Zukunft erkennen können.

<!--

>[!IMPORTANT]
>
>Note a difference in terminology where the sandbox selected from Real-Time CDP is considered a dataset in the UI in Real-Time CDP Collaboration.

-->

### Zuordnen von Feldern {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="Quellfelder"
>abstract="Quellfelder sind Identity-Namespaces und Attribute aus Ihrer bestehenden Implementierung von Real-Time CDP. Sie können diese Zielfeldern zuordnen, die in Real-Time CDP Collaboration definiert sind."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="Zielfelder"
>abstract="Die Zielfelder entsprechen den Übereinstimmungsschlüsseln, die Sie beim Onboarding Ihres Unternehmens ausgewählt haben. Derzeit sind Hash-E-Mails die einzigen unterstützten Übereinstimmungsschlüssel."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="Transformation anwenden"
>abstract="Verwenden Sie beim Importieren von anderen Feldern als *Hash-Feldern* aus Ihrer Quelle diese Option, damit Real-Time CDP Collaboration den Hash anwendet und die einfachen Felder in Hash-Felder umwandelt."

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

![Bildschirm „Felder zuordnen“ mit Quellfeldern, die Zielfeldern zugeordnet sind.](/help/assets/setup/add-manage-audiences/Step-Map-Fields.png)

Im Schritt Felder zuordnen können Sie auswählen, wie alle Identitätsfelder für die Profile, die von der Datenverbindung importiert wurden, den in Ihrer Organisation ausgewählten Übereinstimmungsschlüsseln zugeordnet werden sollen.

>[!TIP]
>
>Sie können demselben Zielfeld mehrere Quellfelder zuordnen. Wenn sich beispielsweise E-Mail-Adressen in zwei separaten Feldern in Experience Platform befinden, können Sie beide dem Zielfeld **[!UICONTROL gehashte E-Mail]** als zwei separate Zeilen zuordnen.

>[!BEGINSHADEBOX]

**[!UICONTROL Source-Felder]** geben an, wie die Identitäten in der Quelle referenziert werden, aus der Sie Daten importieren.

**[!UICONTROL Zielfelder]** geben an, wie die Identitäten in Real-Time CDP Collaboration referenziert werden. Die Werte, die Sie hier auswählen können, entsprechen den Übereinstimmungsschlüsseln, die Sie im Onboarding-Workflow des Unternehmens eingerichtet haben.

Verwenden Sie die **[!UICONTROL Umwandlung anwenden]**, wenn Sie (*gehashte)* aus Ihrer Quelle importieren. In diesem Fall wendet Real-Time CDP Collaboration den Hash-Wert an und wandelt die Felder um. Der von Adobe verwendete Hash-Algorithmus ist SHA256.

>[!ENDSHADEBOX]

Fügen Sie beliebig viele Zuordnungspaare hinzu und klicken Sie auf **[!UICONTROL Weiter]**, um mit dem nächsten Schritt fortzufahren.

<!--

In this step, you can also add any identity crosswalks that you would like to use.

Identity crosswalks will be supported after the beta release.

#### Add identity crosswalk

Use identity crosswalks to connect different identifiers across datasets to enrich your audience data with additional attributes or dimensions. 

TODO add GIF Identity crosswalks screen showing a list of available identity crosswalks with details.

Select **[!UICONTROL Add identity crosswalk]** to see a screen where you can choose from various identity crosswalks that you have previously [imported into Real-Time CDP Collaboration](/help/guide/setup/identity-crosswalk.md#import-crosswalk). Each entry includes details such as the table name, type, description, and creation date.

After selecting the desired crosswalk, use a source field join key to map to the crosswalk table join key. 

>[!NOTE]
>
>After selecting an identity crosswalk, the **[!UICONTROL Add identity crosswalk]** control is greyed out. 

For further reading about identity crosswalks, refer to the [glossary](/help/guide/glossary.md).

-->


<!-- will uncomment this part when Manage use cases part becomes available

### Manage use cases {#manage-use-cases}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_usecases"
>title="Use cases for identities"
>abstract="This control is disabled in the initial release of Real-Time CDP Collaboration"

![Manage use cases screen.](/help/assets/setup/add-manage-audiences/Step-manage-use-cases.png)

For every identity selected in the mapping step, select the use cases that you can use the identity for. Available use cases are: 

* Discover
* Share
* Activate
* Measure

Note that this control is disabled in the initial release of Real-Time CDP Collaboration.

After selecting the desired use cases for each identity, proceed to the next step. 

-->›

### Zeitplan {#schedule}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_audience_expiration"
>title="Ablauf der Zielgruppe"
>abstract="Weitere Details zur Gültigkeit der Zielgruppe."

Planen Sie, wann die Zielgruppen aufgefüllt und aktualisiert werden sollen. Die Zielgruppenzugehörigkeit wird gemäß diesem Zeitplan aktualisiert.

![Bildschirm „Zeitplan“ mit Start- und Enddatum für das Ausfüllen der Zielgruppen.](/help/assets/setup/add-manage-audiences/Step-Schedule.png)

Wählen Sie die Aktualisierungsrate für die Zielgruppen aus. Verfügbare Optionen liegen zwischen einer Aktualisierungsrate von einem Tag und sechs Tagen.

>[!IMPORTANT]
>
>Durch die Anpassung der Aktualisierungshäufigkeit der Zielgruppe können Sie die [Audience-Management-Kreditaktivität](/help/guide/setup/my-activity.md#types-of-activities) verwalten, die pro Aktualisierung der Zielgruppenmitgliedschaft berechnet wird. Dies kann sich auf weniger aktuelle Daten auswirken, die für die Entdeckung von Zielgruppenberichten und die Freigabe und Aktivierung von Zielgruppen verfügbar sind.

![Bildschirm „Zeitplan“ mit verschiedenen Häufigkeitsintervallen zur Aktualisierung der Zielgruppenzugehörigkeit.](/help/assets/setup/add-manage-audiences/Step-Schedule-Set-Frequency.png)

>[!IMPORTANT]
>
>Nach dem Enddatum im Datumsbereich werden alle Zielgruppen, die aus dieser Datenverbindung importiert wurden, nicht mehr aktualisiert. Um die Verbindung zu erneuern, gehen Sie zu [Datenverbindung verwalten](/help/guide/setup/manage-data-connection.md) und legen Sie ein neues Enddatum fest.

### Zielgruppen auswählen {#select-audience}

Nach Auswahl der Zielgruppenquelle wählen Sie bestimmte Zielgruppen aus, die einbezogen werden sollen. Verwenden Sie die Such- und Filteroptionen auf der Seite, um die relevanten Zielgruppen aus Ihrer ausgewählten Datenquelle zu finden.

![Bildschirm „Zielgruppe auswählen“ mit einer Liste der verfügbaren Zielgruppen mit Kontrollkästchen zur Auswahl.](/help/assets/setup/add-manage-audiences/Step-Select-Audience.png)

### Überprüfung

Überprüfen Sie alle Konfigurationen und Einstellungen, bevor Sie das Hinzufügen der Zielgruppe abschließen. Stellen Sie sicher, dass alle Details korrekt sind, und wählen Sie **[!UICONTROL Abschließen]** aus, um den Prozess abzuschließen.

## Anzeigen des Dashboards „Zielgruppen“ {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="Fehlende Identitäten"
>abstract="Die Anzahl der Identitäten ist nach der nächsten Aktualisierung der Datenverbindung verfügbar, die dem konfigurierten Zeitplan folgt. Die erste Aktualisierung erfolgt normalerweise innerhalb von 24 Stunden nach der Einrichtung der Datenverbindung. Laufende Aktualisierungen folgen dem konfigurierten Zeitplan. "

Nach dem Import von Audiences in Real-Time CDP Collaboration können Sie Informationen dazu in einer Dashboard-Ansicht abrufen. Die Standardansicht auf der Seite **[!UICONTROL Meine Zielgruppen]** zeigt alle Zielgruppen an, die derzeit von Ihrem Unternehmen in Real-Time CDP Collaboration importiert wurden.

![Seite „Zielgruppen-Übersicht“ mit allen von einem Advertiser importierten Zielgruppen](/help/assets/setup/add-manage-audiences/audiences-overview.png)

Sie können die folgenden relevanten Informationen zu jeder Zielgruppe anzeigen:

| Element | Beschreibung |
|----------|---------|
| **[!UICONTROL Identitäten]** | Gibt die Anzahl der in dieser Zielgruppe vorhandenen Identitäten an. Beachten Sie Folgendes: Wenn dasselbe Profil zwei oder mehr Identitäten hat und diese Identitäten als Übereinstimmungsschlüssel im Projekt verwendet werden, wird das Profil zweimal in der Zählung angezeigt. |
| **[!UICONTROL Status]** | Gibt an, ob die Zielgruppe aktiv ist und in Projekten verwendet werden kann. Der Status Ausstehend gibt an, dass die Zielgruppe gerade erst importiert wurde und die Zielgruppenmitglieder noch ausgefüllt werden müssen. Die importierten Zielgruppen werden nach der nächsten Aktualisierung der Datenverbindung gemäß dem konfigurierten Zeitplan mit Profilen gefüllt. Die erste Aktualisierung erfolgt normalerweise innerhalb von 24 Stunden nach der Einrichtung der Datenverbindung                                         . |
| **[!UICONTROL Quelle]** | Gibt die Quelle an, aus der diese Zielgruppe importiert wurde. In der aktuellen Version von Real-Time CDP Collaboration ist Adobe Experience Platform die einzige unterstützte Quelle. |
| **[!UICONTROL Datenverbindung]** | Weitere Aufschlüsselungsinformationen darüber, woher diese Zielgruppe importiert wurde. Wenn Sie beispielsweise Zielgruppen aus der Experience Platform-Quelle importieren, werden die einzelnen Sandboxes, auf die Ihr Unternehmen Zugriff hat, als Datenverbindungen betrachtet. |
| **[!UICONTROL Verbindungszugriff]** | Definiert, ob diese Zielgruppe privat oder öffentlich ist. Öffentliche Zielgruppen sind in Überschneidungsberichten zu finden und können für Mitwirkende freigegeben werden. |
| **[!UICONTROL Erstellt]** | Gibt an, wann diese Zielgruppe in Real-Time CDP Collaboration importiert wurde. |
| **[!UICONTROL Zuletzt aktualisiert]** | Gibt das letzte Datum und die letzte Uhrzeit an, zu der ein Aspekt dieser Zielgruppe aktualisiert wurde. |

Wählen **[!UICONTROL Datenverbindungen verwalten]**, um alle eingerichteten Datenverbindungen anzuzeigen und zu bearbeiten.
Klicken Sie auf die Auslassungszeichen und **[!UICONTROL Löschen]**, um die Zielgruppe zu entfernen.
Klicken Sie auf die Auslassungszeichen und **[!UICONTROL Kategorien bearbeiten]**, um der Zielgruppe verschiedene Kategorietags hinzuzufügen. Weitere Informationen finden Sie [ folgenden Abschnitt ](/#categories)Kategorien“.
Wählen Sie den Zielgruppennamen aus, um einzelne Zielgruppen zu überprüfen oder zu bearbeiten.

## Anzeigen einzelner Zielgruppen {#view-individual-audiences}

Die Zielgruppenansicht enthält weitere Informationen zu Ihrer Zielgruppe.

![Anzeigen und Überprüfen einzelner Zielgruppen.](/help/assets/setup/add-manage-audiences/view-inspect-audience.png)

Im Folgenden werden die Metriken beschrieben, die Sie auf diesem Bildschirm anzeigen können:

| Element | Beschreibung |
|----------|---------|
| **[!UICONTROL Status]** | Gibt an, ob die Zielgruppe aktiv ist und in Projekten verwendet werden kann. |
| **[!UICONTROL Quelle]** | Gibt die Quelle an, aus der diese Zielgruppe importiert wurde. In der aktuellen Version von Real-Time CDP Collaboration ist Adobe Experience Platform die einzige unterstützte Quelle. |
| **[!UICONTROL Datenverbindung]** | Weitere Aufschlüsselungsinformationen darüber, woher diese Zielgruppe importiert wurde. Wenn Sie beispielsweise Zielgruppen aus der Experience Platform-Quelle importieren, werden die einzelnen Sandboxes, auf die Ihr Unternehmen Zugriff hat, als Datenverbindungen betrachtet. |
| **[!UICONTROL Zuletzt aktualisiert]** | Gibt das letzte Datum und die letzte Uhrzeit an, zu der ein Aspekt dieser Zielgruppe aktualisiert wurde. |
| **[!UICONTROL Zuletzt aktualisiert von]** | Gibt den Benutzer an, der diese Zielgruppe zuletzt aktualisiert hat. |
| **[!UICONTROL Erstellt]** | Gibt an, wann diese Zielgruppe in Real-Time CDP Collaboration importiert wurde. |
| **[!UICONTROL Erstellt von]** | Gibt den Benutzer an, der die Zielgruppe in Real-Time CDP Collaboration importiert hat. |


Sie können zwei weitere Steuerelemente auf der Seite verwenden, um Zielgruppen zu bearbeiten oder zu entfernen:

* **[!UICONTROL Löschen]**: Entfernen der Zielgruppe aus dem Inventar
* **[!UICONTROL Bearbeiten]**: Bearbeiten von Zielgruppen-Metadaten wie Name oder Beschreibung.

![Anzeigen und Überprüfen einzelner Zielgruppen.](/help/assets/setup/add-manage-audiences/audiences-edit-delete-controls.png)

Weitere Informationen zur Zielgruppe sind in folgenden Widgets verfügbar und können teilweise bearbeitet werden:

![Anzeigen und Überprüfen einzelner Zielgruppen.](/help/assets/setup/add-manage-audiences/audiences-further-info-boxes.png)

* [Identitäten](#identities)
* [Kategorien](#categories)
* [Zugriff auf Verbindungen](#connection-access)
* [Sichtbarkeit von Metadaten](#metadata-visibility)

### Identitäten {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="Identitäten"
>abstract="Sie erhalten eine Aufschlüsselungsansicht der Identitäten, aus denen diese Zielgruppe besteht, sowie eine Gesamtanzahl der Profile mit den entsprechenden Identitäten."

In diesem Abschnitt wird die Anzahl der in der Zielgruppe vorhandenen Profile mit einer der Identitäten angegeben, die Sie beim Import der Zielgruppen angegeben haben. Der Abschnitt enthält auch eine Aufschlüsselung der Identität, sodass Sie feststellen können, welche Identitäten den größten Teil der Zielgruppen-Population ausmachen.

### Kategorien {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="Kategorien"
>abstract="Versehen Sie Ihre Zielgruppen mit Tags, um sie einfach zu organisieren, zu filtern und abzurufen. Sie können eine Zielgruppe mit Tags mehrerer Kategorien versehen und diese Kategorie-Tags anschließend verwenden, um Ihre gewünschten Zielgruppen in anderen Bereichen des Produkts zu filtern."

Um die Organisation, Filterung und den Abruf von Audiences zu vereinfachen, können Sie Ihre Audiences mit Tags versehen. Sie können eine Zielgruppe mit mehreren Kategorien taggen. Anschließend können Sie diese Kategorietags verwenden, um Ihre gewünschten Zielgruppen im Produktbereich [Entdecken](/help/guide/collaborate/discover.md) zu filtern, wenn Sie Berichte zur Zielgruppenüberschneidung ausführen.

### Zugriff auf Verbindungen {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="Zugriff auf Verbindungen"
>abstract="<p>Zielgruppen können drei Typen aufweisen: öffentlich, privat und benutzerdefiniert.</p><p> Ihre Verfügbarkeit für die Verwendung in Projekten mit Mitwirkenden unterscheidet sich je nach Einstellung für den Verbindungszugriff. Sie können den Verbindungszugriff immer von privat in öffentlich ändern. Sobald jedoch eine Zielgruppe für Mitwirkende freigegeben wurde, können Sie diese Einstellung nicht mehr rückgängig machen.</p>"

Wählen Sie aus, ob die Zielgruppe privat für Sie sein soll oder in Verbindungen verwendbar und auffindbar sein soll. Die drei verfügbaren Optionen sind:

* **[!UICONTROL Öffentliche]**. Diese Zielgruppen stehen für die Verwendung in Überschneidungsberichten sowie für die Freigabe und Aktivierung in Verbindungen mit beliebigen Partnern zur Verfügung.
* **[!UICONTROL Private]**. Diese Zielgruppen sind *nicht* verfügbar für die Verwendung in Überschneidungsberichten und für die Freigabe und Aktivierung in Verbindungen mit Mitarbeitern. Obwohl diese Zielgruppe für Mitwirkende nicht zum Anzeigen oder Verwenden verfügbar ist, trägt sie dennoch zur Gesamtpopulation in der Ansicht **[!UICONTROL Alle Zielgruppen]** im Abschnitt [Entdecken und Überschneidungen“ ](/help/guide/collaborate/discover.md#compare-audiences). Ändern Sie die Einstellung in Öffentlich oder Benutzerdefiniert , um die Zielgruppen in Verbindungen mit Partnern zu verwenden.
* **[!UICONTROL Benutzerdefinierte Zielgruppe]**. Diese Zielgruppen sind nur für die Verwendung in Überschneidungsberichten und für die Freigabe und Aktivierung in bestimmten Verbindungen verfügbar. Obwohl diese Zielgruppe nicht für alle Mitwirkenden zum Anzeigen oder Verwenden verfügbar ist, trägt sie dennoch zur Gesamtpopulation in der Ansicht **[!UICONTROL Alle Zielgruppen]** im Abschnitt [Entdecken und Überschneidungen“ ](/help/guide/collaborate/discover.md).

>[!IMPORTANT]
>
>Unabhängig vom Zugriffsstatus (öffentlich, privat oder benutzerdefiniert) trägt die Population einer beliebigen Zielgruppe zur Population **[!UICONTROL Alle Zielgruppen]** in der Ansicht Zielgruppenerkennung - Überschneidung bei. <br> ![Die systemgenerierte Zielgruppe **Alle Zielgruppen** in der Analyse zur Zielgruppenerkennung enthält Zielgruppen mit allen Verbindungszugriffsstatus (öffentlich, privat, benutzerdefiniert).](/help/assets/setup/add-manage-audiences/all-audiences-view.png "Die systemgenerierte Zielgruppe **Alle Zielgruppen** in der **Zielgruppenerkennung**-Überschneidungsanalyse umfasst Zielgruppen mit allen Verbindungszugriffsstatus (öffentlich, privat, benutzerdefiniert)."){width="100" zoomable="yes"}

Die Zielgruppenverfügbarkeit für die Verwendung in Projekten mit Partnern unterscheidet sich je nach Verbindungszugriffseinstellung. Sie können den Verbindungszugriff immer von privat in öffentlich ändern. Sobald jedoch eine Zielgruppe für Mitwirkende freigegeben wurde, können Sie diese Einstellung nicht mehr rückgängig machen.

### Sichtbarkeit von Metadaten {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="Sichtbarkeit von Metadaten"
>abstract="<p>Gibt an, welche der Metadateninformationen von Zielgruppen für andere Organisationen sichtbar sind, bevor sie eine Verbindung zu Ihrer Organisation herstellen. </p> <p> Die **Identitätsanzahl** steuert, ob Ihre Partnerin oder Ihr Partner Identitätsanzahlen für Ihre Zielgruppen anzeigen kann, wenn Überschneidungsberichte auf der Registerkarte „Entdeckung“ angezeigt werden. Die **Zielgruppenüberschneidung in %** steuert, ob Mitwirkende Überschneidungsprozentsätze zwischen ihren Zielgruppen und Ihren Zielgruppen ermitteln können."

>[!NOTE]
>
>Wenn für Ihren Mitarbeiter alle Zielgruppen auf „privat“ eingestellt sind, ist die Ansicht **[!UICONTROL Relevante Zielgruppen]** in den Zielgruppeneinblicken leer. [Weitere Informationen](/help/guide/collaborate/discover.md#relevant-audiences).

Gibt an, welche der Zielgruppen-Metadateninformationen für andere Organisationen sichtbar sind, bevor sie eine Verbindung zu Ihrer Organisation oder in verschiedenen Projektansichten herstellen.

**[!UICONTROL Anzahl der Identitäten anzeigen]** Mit dieser Einstellung wird festgelegt, ob Ihr Partner beim Anzeigen von Überschneidungsberichten auf der Registerkarte [ die Identitätsanzahl für Ihre Zielgruppen anzeigen ](/help/guide/collaborate/discover.md#discover-overlaps).

![Seitenbilder mit deaktivierter und ausgewählter Option „Anzahl der Identitäten anzeigen“.](/help/assets/setup/add-manage-audiences/show-identity-count.png)

**[!UICONTROL Zielgruppenüberschneidung anzeigen %]**: Bei Festlegung auf „true“ können Mitwirkende [Überschneidungsprozentsätze ermitteln](/help/guide/collaborate/discover.md#compare-audiences) zwischen ihren Zielgruppen und der Zielgruppe, die zu Ihnen gehört. In der unten stehenden Aufzeichnung ist diese Konfiguration beispielsweise auf „true“ für die `agora-advertiser-aud3` festgelegt und ein Mitarbeiter kann Überschneidungsprozentsätze mit dieser Zielgruppe anzeigen. Für die Zielgruppe `agora-advertiser-aud1` ist diese Einstellung auf „false“ festgelegt, sodass der Mitarbeiter keine Überschneidungsprozentsätze anzeigen kann.

![Prozentsatz der Zielgruppenüberschneidung für zwei verschiedene Zielgruppen.](/help/assets/setup/add-manage-audiences/audience-overlap-percentage.gif)

## Nächste Schritte

Verwenden Sie nach dem Import von Audiences den Abschnitt [Verbinden](/help/guide/connect/establishing-connections.md), um nach Publishern zu suchen, mit denen Sie eine Verbindung herstellen können, und um mit der Zusammenarbeit an Projekten zu beginnen.
