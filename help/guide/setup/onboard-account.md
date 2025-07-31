---
title: Konfigurieren und Verwalten Ihres Kontos
description: Erfahren Sie, wie Sie verschiedene Aspekte Ihres Kontos in Real-Time CDP Collaboration konfigurieren und verwalten
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 608706d00124372ac59209478ab551a3a6ce0226
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 18%

---

# Konfigurieren und Verwalten Ihres Kontos

{{limited-availability-release-note}}

Erfahren Sie, wie Sie Ihr -Konto in Real-Time CDP Collaboration einrichten, um sich auf Verbindungen mit anderen Mitwirkenden vorzubereiten. In diesem Handbuch wird die Ersteinrichtung Ihres Kontos beschrieben, einschließlich des Hinzufügens von Kontodetails, der Auswahl von Übereinstimmungsschlüsseln und der Verwaltung der Kontoeinstellungen.

![Der Setup-Arbeitsbereich mit einem konfigurierten Konto.](/help/assets/setup/manage-account/my-account.png){zoomable="yes"}

## Einrichten des Kontos {#set-up-account}

Wenn Sie zum ersten Mal auf Collaboration zugreifen, werden Sie aufgefordert, Ihr Konto einzurichten. Dies ist ein einmaliger Prozess, in dem Sie Ihre Kontodetails konfigurieren und Schlüssel abgleichen können. Wenn dies das erste Konto Ihres Unternehmens ist, werden Sie sofort durch den Onboarding-Prozess geleitet, beginnend mit der Einrichtung Ihrer [Kontodetails](#set-up-details).

Um weitere Organisationen hinzuzufügen, gehen Sie in der linken Leiste zu **[!UICONTROL Setup]** und wählen Sie das Symbol Hinzufügen (Symbol ![Hinzufügen) aus.](/help/assets/icons/plus.png)) in der oberen rechten Ecke. Wählen Sie anschließend **[!UICONTROL Konto]** aus.

![Der Arbeitsbereich „Setup“ mit hervorgehobener Registerkarte „Mein Konto“ und hervorgehobener Option „Konto“](/help/assets/setup/manage-account/add-new-account.png){zoomable="yes"}

### Einrichten von Details {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="Kontakt-E-Mail"
>abstract="Geben Sie eine Team- oder rollenbasierte E-Mail-Adresse an, z. B. **collaboration@ihrunternehmen.com**. Persönliche oder individuelle E-Mail-Adressen sollten nicht verwendet werden."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="Verbindungs-Code"
>abstract="Der Verbindungs-Code ist eine eindeutige Kennung für Ihr Konto. Er wird verwendet, um in Real-Time CDP Collaboration Verbindungen zu anderen Mitwirkenden herzustellen."

<!-- Move the above popover to new section for invite on this page when its created -->

Um mit der Konfiguration Ihres Kontos zu beginnen, müssen Sie zunächst die Kontodetails einrichten. Dazu müssen Sie die folgenden Informationen hinzufügen:

* Fügen Sie einen **[!UICONTROL Kontonamen]** hinzu, der Ihre Marke deutlich darstellt.
* Fügen Sie eine **[!UICONTROL Beschreibung]** über Ihre Marke hinzu. Dies ist optional, hilft anderen Mitwirkenden jedoch, Ihre Marke besser zu verstehen.
* Wählen Sie Ihre **[!UICONTROL Rolle]** aus. Sie können zwischen **[!UICONTROL Advertiser]** und **[!UICONTROL Publisher]** wählen. Lesen Sie das [End-to-End](/help/guide/end-to-end-workflow.md)Workflow-Dokument, um Ähnlichkeiten und leichte Unterschiede im Workflow zwischen den beiden Rollentypen der Organisation zu sehen.
<!-- The above will need to be updated when I update things for B2B -->
* Wählen Sie die **[!UICONTROL Branche]** für Ihr Konto aus. Einige Beispiele sind **[!UICONTROL Einzelhandel]**, **[!UICONTROL Telekommunikation]** oder **[!UICONTROL Finanzdienstleistungen]**.
* Die **[!UICONTROL Region]** wird automatisch anhand Ihres Adobe Experience Cloud-Kontos festgelegt. Dies kann nicht jederzeit geändert werden.
* Fügen Sie eine **[!UICONTROL Kontakt-E-Mail]** für Ihr Konto hinzu. Dies sollte eine Team- oder rollenbasierte E-Mail-Adresse sein. Persönliche E-Mail-Adressen sollten nicht angegeben werden.
* Laden Sie ein **[!UICONTROL Logo]** für Ihr Konto hoch. Derzeit werden Bilder vom Typ SVG unterstützt. Dies ist optional, aber das Hochladen eines Logos hilft Ihnen, Ihre Marke in der Collaboration-Benutzeroberfläche visuell darzustellen
* Wählen Sie ein Bild für die Kopfzeile Ihres Kontos aus.

>[!NOTE]
>
>Die meisten dieser Details können zwar jederzeit bearbeitet werden, die **[!UICONTROL Rolle]** kann jedoch nach der Ersteinrichtung nicht mehr bearbeitet werden. Wenn Sie fertig sind, verwenden Sie **[!UICONTROL Weiter]**, um mit der nächsten Seite fortzufahren und die gewünschten Übereinstimmungsschlüssel auszuwählen, die Ihr Unternehmen verwenden wird.

![Der Arbeitsbereich „Konto einrichten“ mit hervorgehobenem Abschnitt „Details“ und hervorgehobener Option „Weiter“.](/help/assets/setup/manage-account/add-account-details.png){zoomable="yes"}

### Einrichten von Übereinstimmungsschlüsseln {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="Übereinstimmungsschlüssel"
>abstract="Übereinstimmungsschlüssel sind Kennungen, die zum zielgruppenübergreifenden Abstimmen der Mitglieder von Zielgruppen aus verschiedenen Datenquellen verwendet werden. Schließen Sie alle Übereinstimmungsschlüssel ein, mit denen Ihre Marke arbeiten kann."

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
>Die Übereinstimmungsschlüssel, die Sie während der Kontoeinrichtung auswählen, bestimmen die verfügbaren Übereinstimmungsschlüssel für die Verbindungen, die Sie mit anderen Partnern erstellen. Während Sie Übereinstimmungsschlüssel während der Verbindungseinrichtung entfernen können, können Sie keine neuen Übereinstimmungsschlüssel hinzufügen. Es ist wichtig, **alle** Übereinstimmungsschlüssel auszuwählen, die Sie in zukünftigen Kampagnen während der Kontoeinrichtung verwenden möchten.

Übereinstimmungsschlüssel wie E-Mail-Adressen, Geräte-IDs oder Kunden-IDs helfen Mitarbeitern bei der Zusammenarbeit, indem sie eine genaue und datenschutzorientierte Datensynchronisation ermöglichen, die eine präzisere Zielgruppen-Zielgruppenbestimmung und -messung ermöglicht.

![Folie mit den verfügbaren Kennungen für die erste Version von Collaboration.](/help/assets/setup/manage-account/available-identifiers.png)

<!-- Eventually replace this image above to match branding better. -->

Wählen Sie die Übereinstimmungsschlüssel aus, die Sie zum Abstimmen der Zielgruppenprofile verwenden möchten. Schließen Sie alle Übereinstimmungsschlüssel ein, mit denen Sie arbeiten können. Planen Sie in Zukunft und wählen Sie die Übereinstimmungsschlüssel aus, die Sie in zukünftigen Kampagnen verwenden werden. Wenn Sie zu einem späteren Zeitpunkt zusätzliche Übereinstimmungsschlüssel für Ihr Konto auswählen müssen, können Sie dies im Workflow [Konto bearbeiten](#edit-account) tun.

Wählen Sie bis zu fünf Übereinstimmungsschlüssel aus, die Sie verwenden möchten. Bei der späteren Einrichtung von Verbindungen können Sie unerwünschte Übereinstimmungsschlüssel entfernen, jedoch keine neuen hinzufügen.

Es gibt drei Arten von verfügbaren Übereinstimmungsschlüsseln:

* Personenbezogene IDs von Erstanbietern
* IDs von Erstanbieter-Geräten
* Partner-IDs

>[!IMPORTANT]
>
>Derzeit wird nur der gehashte E-Mail-Schlüssel als Übereinstimmungsschlüssel unterstützt.

Wenn Sie bereit sind **[!UICONTROL wählen Sie &quot;]**&quot; aus, um den Einrichtungs-Workflow für die Organisation abzuschließen.

![Der Arbeitsbereich Organisation einrichten , wobei der Abschnitt Übereinstimmungsschlüssel angezeigt wird.](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## Konto bearbeiten {#edit-account}

Nachdem Sie Ihr Konto eingerichtet haben, können Sie jederzeit bestimmte Aspekte und Details des Kontos bearbeiten. Um Ihr Konto zu bearbeiten, wählen **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Mein Konto]** des Arbeitsbereichs **[!UICONTROL Setup] aus**.

![Der Arbeitsbereich „Setup“ mit hervorgehobener Registerkarte „Mein Konto“ und hervorgehobener Option „Bearbeiten“.](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

Sie können jetzt Ihre Kontodetails mit Ausnahme von &quot;**[!UICONTROL &quot;]**. Beachten Sie, dass die Region automatisch anhand Ihres Adobe Experience Cloud-Kontos festgelegt wird und nicht jederzeit geändert werden kann.

![Der Dialog Kontodetails bearbeiten.](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

Sie können auch die Übereinstimmungsschlüssel aktualisieren, die Sie ursprünglich beim Onboarding in Ihrer Organisation ausgewählt haben. Wählen Sie **[!UICONTROL Abschnitt]**&#x200B;Übereinstimmungsschlüssel **[!UICONTROL aus,]** weitere gewünschte Übereinstimmungsschlüssel hinzuzufügen.

![Der Arbeitsbereich „Setup“ mit hervorgehobener Option „Bearbeiten“ im Abschnitt „Übereinstimmungsschlüssel“ des Kontos.](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

## Nächste Schritte

Nachdem Sie Ihre Konten eingerichtet haben, können Sie [Zielgruppen](/help/guide/setup/onboard-audiences.md) in Real-Time CDP Collaboration beziehen.
