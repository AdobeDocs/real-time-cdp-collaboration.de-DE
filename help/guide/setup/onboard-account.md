---
title: Konfigurieren und Verwalten Ihres Kontos
description: Erfahren Sie, wie Sie verschiedene Aspekte Ihres Kontos in Real-Time CDP Collaboration konfigurieren und verwalten
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
TQID: https://experienceleague.adobe.com/PRmSkRSE2tQ-5t5hHKzDAGrkF6-irmZid2Akq6-PQv8
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1393
ht-degree: 13%

---

# Konfigurieren und Verwalten Ihres Kontos

{{limited-availability-release-note}}

Erfahren Sie, wie Sie Ihr -Konto in Real-Time CDP Collaboration einrichten, um sich auf Verbindungen mit anderen Mitwirkenden vorzubereiten. In diesem Handbuch wird die Ersteinrichtung Ihres Kontos beschrieben, einschließlich des Hinzufügens von Kontodetails, der Auswahl von Übereinstimmungsschlüsseln und der Verwaltung der Kontoeinstellungen.

![Der Setup-Arbeitsbereich mit einem konfigurierten Konto.](/help/assets/setup/manage-account/my-account.png){zoomable="yes"}

## Einrichten des Kontos {#set-up-account}

Wenn Sie zum ersten Mal auf Collaboration zugreifen, werden Sie aufgefordert, Ihr Konto einzurichten. Dies ist ein einmaliger Prozess, in dem Sie Ihre Kontodetails konfigurieren und Schlüssel abgleichen können. Wenn dies das erste Konto Ihres Unternehmens ist, werden Sie sofort durch den Onboarding-Prozess geleitet, beginnend mit der Einrichtung Ihrer [Kontodetails](#set-up-details).

Um weitere Organisationen hinzuzufügen, gehen Sie in der linken Leiste zu **[!UICONTROL Setup]** und wählen Sie das Symbol zum Hinzufügen aus (![Symbol hinzufügen.](/help/assets/icons/plus.png)) in der oberen rechten Ecke. Wählen Sie anschließend **[!UICONTROL Konto]** aus.

![Der Arbeitsbereich „Setup“ mit hervorgehobener Registerkarte „Mein Konto“ und hervorgehobener Option „Konto“](/help/assets/setup/manage-account/add-new-account.png){zoomable="yes"}

### Einrichten von Details {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="Kontakt-E-Mail"
>abstract="Bitte eine Team- oder rollenbasierte E-Mail-Adresse angeben, z. B. **collaboration@yourcompany.com**. Persönliche oder individuelle E-Mail-Adressen sollten nicht verwendet werden."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="Verbindungs-Code"
>abstract="Der Verbindungs-Code ist eine eindeutige Kennung für Ihr Konto. Er wird verwendet, um in Real-Time CDP Collaboration Verbindungen zu anderen Mitwirkenden herzustellen."

Um mit der Konfiguration Ihres Kontos zu beginnen, müssen Sie zunächst die Kontodetails einrichten. Dazu müssen Sie die folgenden Informationen hinzufügen:

* Fügen Sie einen **[!UICONTROL Kontonamen]** hinzu, der Ihre Marke deutlich darstellt.
* Fügen Sie eine **[!UICONTROL Beschreibung]** über Ihre Marke hinzu. Dies ist optional, hilft anderen Mitwirkenden jedoch, Ihre Marke besser zu verstehen.
* Wählen Sie Ihre **[!UICONTROL Rolle]** aus. Sie können zwischen **[!UICONTROL Advertiser]** und **[!UICONTROL Publisher]** wählen. Lesen Sie das [Rollen](/help/guide/overview/roles.md)-Handbuch, um Ähnlichkeiten und leichte Unterschiede im Workflow zwischen den beiden Kontorollentypen zu sehen.
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
>abstract="Übereinstimmungsschlüssel sind Kennungen, die zum Abstimmen der Profile von Zielgruppen aus verschiedenen Datenquellen verwendet werden. Schließen Sie alle Übereinstimmungsschlüssel ein, mit denen Ihre Marke arbeiten kann."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_setup_match_keys"
>title="Übereinstimmungsschlüssel"
>abstract=""

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="Personenbezogene IDs aus erster Hand"
>abstract="Personenbezogene IDs aus erster Hand wie Hash-E-Mail-Adressen, Hash-Telefonnummern oder CRM-IDs sind direkt mit einem einzelnen Profil verbunden."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="IDs von Erstanbieter-Geräten"
>abstract="Geräte-IDs von Erstanbietern wie ECID oder IP-Adressen sind direkt mit Geräten verbunden, die möglicherweise von mehreren Personen gemeinsam genutzt werden können."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="Unterstützte Partner-IDs"
>abstract="Partner-IDs sind Kennungen, die von externen Partnern zur Abstimmung von Zielgruppen bereitgestellt werden. Partner-IDs sind nicht direkt mit einem einzelnen Profil verbunden."

![Unterstützte Übereinstimmungsschlüssel.](/help/assets/setup/manage-account/match-keys.png){zoomable="yes"}

>[!IMPORTANT]
>
>Die Übereinstimmungsschlüssel, die Sie während der Kontoeinrichtung auswählen, bestimmen die verfügbaren Übereinstimmungsschlüssel innerhalb Ihrer Verbindungen. Während Sie [unerwünschte Übereinstimmungsschlüssel entfernen](../connect/establishing-connections.md#connection-settings) während der Verbindungseinrichtung können Übereinstimmungsschlüssel nicht hinzugefügt werden, nachdem eine Verbindung hergestellt wurde. Es ist wichtig, dass Sie **alle** Übereinstimmungsschlüssel auswählen, die Sie in zukünftigen Kampagnen während der Kontoeinrichtung verwenden möchten.

Match-Schlüssel helfen Mitarbeitern bei der Zusammenarbeit, indem sie eine genaue und datenschutzorientierte Datensynchronisation ermöglichen, was eine präzisere Zielgruppenbestimmung und -messung ermöglicht. Die bei der Kontoeinrichtung ausgewählten Übereinstimmungsschlüssel bestimmen, welche Übereinstimmungsschlüssel in zukünftigen Verbindungen verfügbar sind. Sie werden auch verwendet, [&#x200B; Felder &#x200B;](./onboard-audiences.md#map-fields) Ihrer Datenverbindung den Zielfeldern in Collaboration beim Sourcing von Zielgruppen zuzuordnen.

Wählen Sie die Übereinstimmungsschlüssel aus, die Sie zum Abstimmen der Zielgruppenprofile verwenden möchten. Planen Sie für die Zukunft und fügen Sie alle Übereinstimmungsschlüssel hinzu, mit denen Sie arbeiten können und die Sie in zukünftigen Kampagnen voraussichtlich verwenden werden. Wenn Sie zu einem späteren Zeitpunkt zusätzliche Übereinstimmungsschlüssel für Ihr Konto auswählen müssen, können Sie dies im Workflow [Konto bearbeiten](#edit-account) tun. Übereinstimmungsschlüssel, die nach der Ersteinrichtung hinzugefügt wurden, stehen jedoch nicht zur Verwendung in vorhandenen Verbindungen zur Verfügung.

#### Unterstützte Übereinstimmungsschlüssel {#supported-match-keys}

Collaboration unterstützt drei Arten von Übereinstimmungsschlüsseln: Erstanbieter-Personen-IDs, Erstanbieter-Geräte-IDs und Partner-IDs. Alle Übereinstimmungsschlüssel müssen die folgenden Anforderungen erfüllen:

* Übereinstimmungsschlüssel müssen **gekürzt**, **kleingeschrieben**
* Hash-Übereinstimmungsschlüssel müssen **SHA256-hashed** sein.
* Wenn Sie Hash-Werte mit Großbuchstaben angeben, wandelt Collaboration diese automatisch in Kleinbuchstaben um.
* Wenn Ihre Quelle **Klartext-IDs** enthält, verwenden Sie die Option **[!UICONTROL Umwandlung anwenden]** während Ihrer [Datenverbindungseinrichtung](./manage-data-connection.md#match-keys), um Hashing anzuwenden. Diese Option ist nur verfügbar, wenn Zielgruppen aus Experience Platform bezogen werden, und wird für Cloud-basierte Quellen nicht unterstützt.

##### Personenbezogene IDs aus erster Hand

First-Party-Personen-IDs sind direkt mit einem einzelnen Profil verbunden. Derzeit unterstützte IDs sind:

* **[!UICONTROL Hash-E-Mail]**
* **[!UICONTROL Hash-Telefon]**
* **[!UICONTROL CRM-IDs]**
* **[!UICONTROL Treue-IDs]**
<!-- * **[!UICONTROL Custom ID]**: Custom identifiers -->

##### IDs von Erstanbieter-Geräten

Erstanbieter-Geräte-IDs sind Kennungen, die mit einem bestimmten Gerät verbunden sind. Derzeit unterstützte IDs sind:

* **[!UICONTROL Hash IPv4]**: Hash-IPv4-Adressen
* **[!UICONTROL IDFA]**: Die Kennung für Advertiser (IDFA), die in Apple iOS-Geräten verwendet werden
* **[!UICONTROL GAID]**: Google Advertiser-ID, die auf Android-Geräten verwendet wird

##### Partner-IDs

Partner-IDs sind Kennungen, die von externen Partnern zur Abstimmung von Zielgruppen bereitgestellt werden. Derzeit unterstützte IDs sind:

* **[!UICONTROL AdFixus-ID]**

>[!NOTE]
>
>Die Integration von Adobe mit [!DNL AdFixus] ordnet die eindeutigen [!UICONTROL AdFixus-IDs] für jedes Konto einem gemeinsamen Adobe-kodierten Format zu. Diese Zuordnungen werden verwendet, um Überschneidungen zwischen Partnern zu identifizieren. Beim Aktivieren von Zielgruppen mit **[!UICONTROL AdFixus ID]** werden die ursprünglichen IDs verwendet. Das Adobe-kodierte Format verlässt Collaboration nie.

Bei Auswahl von **[!UICONTROL AdFixus ID]** müssen Sie im Abschnitt **[!UICONTROL Kontoanmeldeinformationen]** die entsprechende ID von Ihrem externen Partner angeben. Diese Option ist nur nach *Umschalten auf „AdFixus **[!UICONTROL ID* verfügbar]**. Geben Sie Ihre AdFixus-ID in das Feld **[!UICONTROL Konto-ID]** ein. Achten Sie darauf, den Wert auf Genauigkeit zu überprüfen.

![The Match keys dialog with AdFixus ID toggled on and the Account credentials section highlighted.](/help/assets/setup/manage-account/adfixus-settings.png){zoomable="yes"}

After you&#39;ve selected all desired match keys, select **[!UICONTROL Complete]** to finish the account setup workflow.

![The Set up account workspace with the Match keys section displayed.](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## Edit account {#edit-account}

After setting up your account, you can edit the details and match keys at anytime.

### Details bearbeiten {#edit-details}

You can edit most details of your account at any time, with the exception of the **[!UICONTROL Role]**. The region is automatically set based on your Adobe Experience Cloud account and cannot be changed.

To edit your account, select **[!UICONTROL Edit]** in the **[!UICONTROL My account]** section of the **[!UICONTROL Setup]** workspace.

![The Setup workspace with the My account tab and Edit option highlighted.](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

You can now edit your account details. Update any fields you want to change and then select **[!UICONTROL Save]** to confirm the changes.

![The Edit account details dialog.](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

### Übereinstimmungsschlüssel bearbeiten {#edit-match-keys}

You can also update the match keys that you initially selected when creating your account. These match keys will determine the match keys available to future connections.

Select **[!UICONTROL Edit]** in the **[!UICONTROL Match keys]** section.

![The Setup workspace with the Edit option highlighted within the account&#39;s Match keys section.](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

The **[!UICONTROL Match keys]** dialog appears. Toggle on any match keys, or update your **[!UICONTROL Account ID]** for your [!UICONTROL AdFixus ID&#39;s],and then select **[!UICONTROL Save]** to confirm the changes.

>[!IMPORTANT]
>
>Changing your [!UICONTROL AdFixus ID] will not trigger a [data sketch](../glossary.md#sketches) refresh for your existing data connections using the match key. Once your data has been sketched, any changes to your [!UICONTROL AdFixus ID] will not be reflected until your next audience refresh following your [data connection schedule](./manage-data-connection.md#scheduling) settings. If you require changes before your next refresh, you can delete and recreate your data connection.
>
>At this time, match keys cannot be removed once added to your account.

![The Match keys dialog with the Save option highlighted.](/help/assets/setup/manage-account/match-key-dialog.png){zoomable="yes"}

A success dialog confirms that your account&#39;s match keys are updated successfully.

![A success dialog confirming your account&#39;s match keys are updated successfully.](/help/assets/setup/manage-account/match-key-updated-successfully.png){zoomable="yes"}

## Nächste Schritte

Nachdem Sie Ihre Konten eingerichtet haben, können Sie [Zielgruppen](/help/guide/setup/onboard-audiences.md) in Real-Time CDP Collaboration beziehen.
