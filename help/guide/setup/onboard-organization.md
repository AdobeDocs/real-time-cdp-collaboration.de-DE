---
title: Onboarding und Verwalten von Organisationen
description: Erfahren Sie, wie Sie verschiedene Aspekte Ihres Unternehmens in Real-Time CDP Collaboration integrieren und verwalten können.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 860138b95abc4d6af94bbbf722cf498463570c1b
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 16%

---

# Onboarding und Verwalten Ihres Unternehmens

{{limited-availability-release-note}}

Erfahren Sie, wie Sie Ihr Unternehmen in Real-Time CDP Collaboration integrieren und verschiedene Aspekte Ihres Unternehmens verwalten können. Auf dieser Seite werden die Schritte zum Onboarding eines Unternehmens in Adobe Real-Time CDP Collaboration beschrieben, einschließlich der Festlegung der Übereinstimmungsschlüssel, bevorzugten Identitäten und mehr Optionen.

![Der Einrichtungsarbeitsbereich des Unternehmens, in dem die aktuellen Einstellungen angezeigt werden.](/help/assets/setup/manage-organization/my-organization.png){zoomable="yes"}

## Erstmaliges Einrichten der Organisation

Zunächst müssen Sie die Details Ihrer Organisation und Organisation einrichten. Wenn dies Ihre erste Organisation ist, werden Sie sofort durch den Onboarding-Prozess geleitet, beginnend mit der Einrichtung Ihrer [Kontodetails](#set-up-details).

Um weitere Organisationen hinzuzufügen, gehen Sie in der linken Leiste zu **[!UICONTROL Setup]** und wählen Sie das Symbol Hinzufügen (Symbol ![Hinzufügen) aus.](/help/assets/icons/plus.png)) in der oberen rechten Ecke. Wählen Sie anschließend **[!UICONTROL Konto]** aus.

![Der Arbeitsbereich „Setup“ mit hervorgehobener Option „Konto“.](/help/assets/setup/manage-organization/add-new-account.png){zoomable="yes"}

### Einrichten von Details {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="Kontakt-E-Mail"
>abstract="Geben Sie eine Team- oder rollenbasierte E-Mail-Adresse an, z. B. `collaboration@yourcompany.com`. Persönliche oder individuelle E-Mail-Adressen sollten nicht verwendet werden."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="Verbindungs-Code"
>abstract="Der Verbindungs-Code ist eine eindeutige Kennung für Ihre Organisation. Sie wird verwendet, um Verbindungen zu anderen Organisationen in Real-Time CDP Collaboration herzustellen."

<!-- Move the above to new section for invite on this page when its created -->

Um mit dem Onboarding Ihrer Organisation zu beginnen, müssen Sie zunächst die Organisationsdetails einrichten. Dazu müssen Sie die folgenden Informationen hinzufügen:

* Fügen Sie einen **[!UICONTROL Organisationsnamen]** für Ihr Unternehmen hinzu.
* Fügen Sie eine **[!UICONTROL Beschreibung]** über Ihr Unternehmen hinzu.
* Wählen Sie Ihre **[!UICONTROL Unternehmensrolle]** aus. Sie können zwischen **[!UICONTROL Advertiser]** und **[!UICONTROL Publisher]** wählen. Lesen Sie das [End-to-End](/help/guide/end-to-end-workflow.md)Workflow-Dokument, um Ähnlichkeiten und leichte Unterschiede im Workflow zwischen den beiden Rollentypen der Organisation zu sehen.
* Wählen Sie die **[!UICONTROL Branche]** für Ihr Unternehmen aus. Einige Beispiele sind **[!UICONTROL Einzelhandel]**, **[!UICONTROL Telekommunikation]** oder **[!UICONTROL Finanzdienstleistungen]**.
* Wählen Sie die **[!UICONTROL Region]** für Ihre Organisation aus. In der aktuellen Version des Produkts ist **[!UICONTROL Nordamerika]** die voreingestellte Standardauswahl.
* Fügen Sie eine **[!UICONTROL Kontakt-E-Mail]** für Ihre Organisation hinzu. Dies sollte eine Team- oder rollenbasierte E-Mail-Adresse sein. Persönliche E-Mail-Adressen sollten nicht angegeben werden.
* Laden Sie ein **[!UICONTROL Logo]** für Ihr Unternehmen hoch. Derzeit werden Bilder vom Typ SVG unterstützt.
* Wählen Sie ein Bild für die Kopfzeile Ihres Unternehmens aus.

>[!NOTE]
>
>Die meisten dieser Details können zwar jederzeit bearbeitet werden, aber **[!UICONTROL Rolle]** und **[!UICONTROL Region]** können nach der Ersteinrichtung nicht mehr bearbeitet werden.

![Der Arbeitsbereich Organisation einrichten , wobei der Abschnitt Details angezeigt wird.](/help/assets/setup/manage-organization/add-organization-details.png){zoomable="yes"}

Wenn Sie fertig sind, verwenden Sie **[!UICONTROL Weiter]**, um mit der nächsten Seite fortzufahren und die gewünschten Übereinstimmungsschlüssel auszuwählen, die Ihr Unternehmen verwenden wird.

### Einrichten von Übereinstimmungsschlüsseln {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="Übereinstimmungsschlüssel"
>abstract="Übereinstimmungsschlüssel sind Kennungen, die zum zielgruppenübergreifenden Abstimmen der Mitglieder von Zielgruppen aus verschiedenen Datenquellen verwendet werden. Schließen Sie alle Übereinstimmungsschlüssel ein, mit denen Ihr Unternehmen arbeiten kann."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="Personenbezogene IDs von Erstanbietern"
>abstract="Personenbezogene IDs von Erstanbietern wie Hash-E-Mail-Adressen oder Telefonnummern sind direkt mit einem einzelnen Profil verbunden. Die derzeit unterstützten IDs sind Hash-E-Mails und Telefonnummern."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="IDs von Erstanbieter-Geräten"
>abstract="Geräte-IDs von Erstanbietern wie ECIDs oder IP-Adressen sind direkt mit Geräten verbunden, die von mehreren Personen gemeinsam genutzt werden können. IPv4 ist die einzige derzeit unterstützte Erstanbieter-Geräte-ID."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="Unterstützte Partner-IDs"
>abstract="Mit Profilen verknüpfte Partner-IDs erweitern die Reichweite auf ein bestimmtes Profil."

>[!IMPORTANT]
>
>Die Übereinstimmungsschlüssel, die Sie bei der Einrichtung der Organisation auswählen, bestimmen die verfügbaren Übereinstimmungsschlüssel für die Verbindungen, die Sie mit anderen Organisationen erstellen. Während Sie Übereinstimmungsschlüssel während der Verbindungseinrichtung entfernen können, können Sie später keine neuen Übereinstimmungsschlüssel hinzufügen. Es ist wichtig, alle Übereinstimmungsschlüssel auszuwählen, die Sie in zukünftigen Kampagnen während der Einrichtung der Organisation verwenden möchten.

Übereinstimmungsschlüssel wie E-Mail-Adressen, Geräte-IDs oder Kunden-IDs helfen Advertisern und Publishern bei der Zusammenarbeit, indem sie eine genaue und datenschutzorientierte Datensynchronisation ermöglichen, was eine präzisere Zielgruppen-Zielgruppenbestimmung und -messung ermöglicht.

![Folie mit den verfügbaren Kennungen für die erste Version von Real-Time CDP Collaboration.](/help/assets/setup/manage-organization/available-identifiers.png)

Wählen Sie die Übereinstimmungsschlüssel aus, die Sie zum Abgleichen von Mitgliedern der Publisher- und Advertiser-Zielgruppen verwenden möchten. Schließen Sie alle Übereinstimmungsschlüssel ein, mit denen Ihre Firma arbeiten kann. Planen Sie für die Zukunft und wählen Sie die Übereinstimmungsschlüssel aus, die Sie in zukünftigen Publisher-Advertiser-Kampagnen voraussichtlich verwenden werden. Wenn Sie zusätzliche Übereinstimmungsschlüssel für Ihre Organisation auswählen müssen, können Sie dies auch zu einem späteren Zeitpunkt im Workflow [Organisation bearbeiten](#edit-organization) tun.

![Der Arbeitsbereich Organisation einrichten , wobei der Abschnitt Übereinstimmungsschlüssel angezeigt wird.](/help/assets/setup/manage-organization/add-organization-match-keys.png){zoomable="yes"}

Wählen Sie bis zu fünf Übereinstimmungsschlüssel aus, die Sie verwenden möchten. Bei der späteren Einrichtung von Verbindungen können Sie unerwünschte Übereinstimmungsschlüssel entfernen, jedoch keine neuen hinzufügen.

Verfügbare Übereinstimmungsschlüssel in Real-Time CDP Collaboration können drei Typen aufweisen:

* Personenbezogene IDs von Erstanbietern
* IDs von Erstanbieter-Geräten
* Partner-IDs

Die verfügbaren Übereinstimmungsschlüssel für die erste Version von Real-Time CDP Collaboration sind:

* Gehashte E-Mail

Wenn Sie bereit sind **[!UICONTROL wählen Sie &quot;]**&quot; aus, um den Einrichtungs-Workflow für die Organisation abzuschließen.

## Organisation bearbeiten {#edit-organization}

Nach der erstmaligen Einrichtung Ihrer Organisation können Sie jederzeit bestimmte Aspekte und Details der Organisation bearbeiten. Um Ihre Organisation zu bearbeiten, wählen **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Meine Organisation]** des Arbeitsbereichs **[!UICONTROL Setup] aus**.

![Der Arbeitsbereich „Setup“ mit hervorgehobener Registerkarte „Meine Organisation“ und hervorgehobener Option „Bearbeiten“.](/help/assets/setup/manage-organization/edit-organization.png){zoomable="yes"}

Sie können jetzt die Details Ihrer Organisation bearbeiten, mit Ausnahme von **[!UICONTROL Rolle]** und **[!UICONTROL Region]**.

![Der Dialog Organisationsdetails bearbeiten.](/help/assets/setup/manage-organization/editable-options.png){zoomable="yes"}

Sie können auch die Übereinstimmungsschlüssel aktualisieren, die Sie ursprünglich beim Onboarding in Ihrer Organisation ausgewählt haben. Wählen Sie **[!UICONTROL Abschnitt]**&#x200B;Übereinstimmungsschlüssel **[!UICONTROL aus,]** weitere gewünschte Übereinstimmungsschlüssel hinzuzufügen.

![Der Arbeitsbereich „Setup“ mit hervorgehobener Option „Bearbeiten“ im Abschnitt „Übereinstimmungsschlüssel“ des Unternehmens.](/help/assets/setup/manage-organization/edit-match-keys.png){zoomable="yes"}

## Nächste Schritte

Nach der Einrichtung Ihres Unternehmens können Sie Zielgruppen [ Real-Time CDP Collaboration ](/help/guide/setup/onboard-audiences.md).
