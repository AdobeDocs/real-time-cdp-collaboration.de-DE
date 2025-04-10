---
title: Onboarding und Verwalten von Organisationen
description: Erfahren Sie, wie Sie verschiedene Aspekte Ihres Unternehmens in Real-Time CDP Collaboration integrieren und verwalten können.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 1%

---

# Onboarding und Verwalten von Organisationen

{{limited-availability-release-note}}

Erfahren Sie, wie Sie Ihr Unternehmen in Real-Time CDP Collaboration integrieren und verschiedene Aspekte Ihres Unternehmens verwalten können. Auf dieser Seite werden die Schritte zum Onboarding eines Unternehmens in Adobe Real-Time CDP Collaboration beschrieben, einschließlich der Festlegung der Übereinstimmungsschlüssel, bevorzugten Identitäten und mehr Optionen.

![Setup-Seite](/help/assets/setup/manage-organization/my-organization.png){zoomable="yes"}

## Erstmaliges Einrichten der Organisation

Zunächst müssen Sie die Details Ihrer Organisation und Organisation einrichten. Navigieren Sie **[!UICONTROL Setup]** in der linken Leiste, klicken Sie auf das Symbol **+** in der oberen rechten Ecke und wählen Sie **[!UICONTROL Konto]**.

>[!TIP]
>
>Nachdem Sie ein anfängliches Konto eingerichtet haben, mit dem Sie arbeiten können, können Sie denselben Workflow verwenden, um zusätzliche Konten innerhalb derselben Organisation einzurichten.

![Konto auswählen, um Real-Time CDP Collaboration eine neue Organisation hinzuzufügen](/help/assets/setup/manage-organization/add-new-account.png){zoomable="yes"}

Der Workflow zum Einrichten Ihrer Organisation umfasst die beiden folgenden Seiten:

* [Details einrichten](#set-up-details)
* [Einrichten von Übereinstimmungsschlüsseln](#set-up-match-keys)

>[!IMPORTANT]
>
>Alle *Übereinstimmungsschlüssel* die Sie auf Organisationsebene auswählen, sickern dann in der ](/help/guide/collaborate/manage-projects.md) zwischen Werbetreibenden und Publishern bis zur [Projektebene) durch. Auf Projektebene können Sie dann alle Übereinstimmungsschlüssel entfernen, aber Sie können *nicht* zusätzliche Schlüssel hinzufügen, die auf Organisationsebene in diesem Bildschirm nicht ausgewählt wurden.

### Details einrichten {#set-up-details}

![Die Schritte Details und Anwendungsfälle zum Einrichten einer Organisation](/help/assets/setup/manage-organization/add-organization-details.png){zoomable="yes"}

1. Fügen Sie einen **[!UICONTROL Organisationsnamen]** für Ihr Unternehmen hinzu.
2. Fügen Sie eine **[!UICONTROL Beschreibung]** über Ihr Unternehmen hinzu.
3. Wählen Sie Ihre **[!UICONTROL Unternehmensrolle]** aus. Sie können zwischen **[!UICONTROL Advertiser]** und **[!UICONTROL Publisher]** wählen. Lesen Sie das [End-to-End](/help/guide/end-to-end-workflow.md)Workflow-Dokument, um Ähnlichkeiten und leichte Unterschiede im Workflow zwischen den beiden Rollentypen der Organisation zu sehen.
4. Wählen Sie die **[!UICONTROL Branche]** für Ihr Unternehmen aus. Einige Beispiele sind **[!UICONTROL Einzelhandel]**, **[!UICONTROL Telekommunikation]** oder **[!UICONTROL Finanzdienstleistungen]**.
5. Wählen Sie die **[!UICONTROL Region]** für Ihre Organisation aus. In der aktuellen Version des Produkts ist **[!UICONTROL Nordamerika]** die voreingestellte Standardauswahl.
6. <span class="preview"> Nur Publisher</span>: Beim Einrichten einer Publisher-Organisation müssen Sie lesen und bestätigen, dass Sie von Werbetreibenden im Publisher-Katalog gefunden werden können.
   ![Publisher-spezifische Opt-in-Nachricht.](/help/assets/setup/manage-organization/publisher-specific-optin-message.png){zoomable="yes"}
7. Laden Sie ein **[!UICONTROL Logo]** für Ihr Unternehmen hoch. Derzeit werden Bilder vom Typ SVG unterstützt.
8. Wählen Sie ein Bild für die Kopfzeile Ihres Unternehmens aus.

Wenn Sie mit Ihrer Auswahl zufrieden sind, verwenden Sie **[!UICONTROL Weiter]**, um mit der nächsten Seite fortzufahren, und wählen Sie die gewünschten Übereinstimmungsschlüssel aus, die Ihre Organisation verwenden soll.

### Übereinstimmungsschlüssel einrichten {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="Übereinstimmungsschlüssel"
>abstract="Übereinstimmungsschlüssel sind Kennungen, die zum Abgleichen von Mitgliedern über Zielgruppen hinweg aus verschiedenen Datenquellen hinweg verwendet werden. Schließen Sie alle Übereinstimmungsschlüssel ein, mit denen Ihre Firma arbeiten kann."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="First-Party-Personen-IDs"
>abstract="First-Party-Personen-IDs wie Hash-E-Mail-Adressen oder Telefonnummern sind direkt mit einem einzelnen Profil verbunden. Derzeit unterstützte IDs sind gehashte E-Mails und Telefonnummern."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="IDs von Erstanbieter-Geräten"
>abstract="Erstanbieter-Geräte-IDs wie ECID- oder IP-Adressen sind direkt mit Geräten verbunden, die von mehreren Personen gemeinsam genutzt werden können. IPv4 ist die einzige derzeit unterstützte First-Party-Geräte-ID."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="Unterstützte Partner-IDs"
>abstract="Mit Profilen verknüpfte Partner-IDs erweitern die Reichweite auf ein bestimmtes Profil."

Übereinstimmungsschlüssel wie E-Mail-Adressen, Geräte-IDs oder Kunden-IDs helfen Advertisern und Publishern bei der Zusammenarbeit, indem sie eine genaue und datenschutzkonforme Datensynchronisation ermöglichen, was eine präzisere Zielgruppen-Zielgruppenbestimmung und -messung ermöglicht.

![Folie mit den verfügbaren Kennungen für die erste Version von Real-Time CDP Collaboration.](/help/assets/setup/manage-organization/available-identifiers.png)

Wählen Sie die Übereinstimmungsschlüssel aus, die Sie zum Abgleichen von Mitgliedern der Publisher- und Advertiser-Zielgruppen verwenden möchten. Schließen Sie alle Übereinstimmungsschlüssel ein, mit denen Ihre Firma arbeiten kann. Planen Sie für die Zukunft und wählen Sie die Übereinstimmungsschlüssel aus, die Sie in zukünftigen Publisher-Advertiser-Kampagnen voraussichtlich verwenden werden. Wenn Sie zusätzliche Übereinstimmungsschlüssel für Ihre Organisation auswählen müssen, können Sie dies auch zu einem späteren Zeitpunkt im Workflow [Organisation bearbeiten](#edit-organization) tun.

![Auswahlschritt für Übereinstimmungsschlüssel.](/help/assets/setup/manage-organization/add-organization-match-keys.png){zoomable="yes"}

Wählen Sie bis zu fünf Übereinstimmungsschlüssel aus, die Sie verwenden möchten. Bei der späteren Einrichtung von Verbindungen können Sie unerwünschte Übereinstimmungsschlüssel entfernen, jedoch keine neuen hinzufügen. Legen Sie den Schwellenwert für die Identitätsanzahl (Mindestanzahl) für jeden ausgewählten Übereinstimmungsschlüssel fest. Übereinstimmende Schlüssel mit weniger als der minimalen Anzahl werden für einige Anwendungsfälle nicht in den Identitätsaufschlüsselungen angezeigt.

Verfügbare Übereinstimmungsschlüssel in Real-Time CDP Collaboration können drei Typen aufweisen:

* First-Party-Personen-IDs
* IDs von Erstanbieter-Geräten
* Partner-IDs

Die verfügbaren Übereinstimmungsschlüssel für die erste Version von Real-Time CDP Collaboration sind:

* Gehashte E-Mail

<!--

not available in the Limited GA release

* Hashed phone
* IPv4

-->

Wenn Sie bereit sind **[!UICONTROL wählen Sie &quot;]**&quot; aus, um den Einrichtungs-Workflow für die Organisation abzuschließen.

## Organisation bearbeiten {#edit-organization}

Nach der erstmaligen Einrichtung Ihrer Organisation können Sie jederzeit bestimmte Aspekte und Details der Organisation bearbeiten. Um Ihre Organisation zu bearbeiten, wählen Sie **[!UICONTROL Bearbeiten]** in der Ansicht **[!UICONTROL Meine Organisation]** aus.

![Organisationssteuerung bearbeiten hervorgehoben.](/help/assets/setup/manage-organization/edit-organization.png){zoomable="yes"}

An dieser Stelle können Sie den Organisationsnamen, die Beschreibung, das Logo und das Profilbild der Organisation aktualisieren.

![Bearbeitbare Optionen für Organisationen.](/help/assets/setup/manage-organization/editable-options.png){zoomable="yes"}

Sie können auch die Übereinstimmungsschlüssel aktualisieren, die Sie ursprünglich beim Onboarding in Ihrer Organisation ausgewählt haben, sowie den Mindestschwellenwert für Identitäten, die Übereinstimmungsschlüsseln entsprechen, damit sie in Zielgruppenüberschneidungen und anderen Produktbereichen sichtbar und verwendbar sind. Wählen Sie **[!UICONTROL Bearbeiten]** auf der Registerkarte **[!UICONTROL Übereinstimmungsschlüssel]** aus, um weitere gewünschte Übereinstimmungsschlüssel hinzuzufügen oder die Identitätsschwellenwerte zu aktualisieren.

![Übereinstimmungsschlüssel bearbeiten](/help/assets/setup/manage-organization/edit-match-keys.png){zoomable="yes"}

## Nächste Schritte

Nach der Einrichtung Ihres Unternehmens können Sie Zielgruppen [ Real-Time CDP Collaboration ](/help/guide/setup/onboard-audiences.md).
