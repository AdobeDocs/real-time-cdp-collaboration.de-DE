---
title: Konfigurieren von Adobe Experience Platform als Ziel
description: Erfahren Sie, wie Sie Adobe Experience Platform as a -Ziel in Real-Time CDP Collaboration konfigurieren und verwalten.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: c36814b8dc975b5ea243688981481de49a8219fd
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# Konfigurieren von Adobe Experience Platform als Ziel

{{limited-availability-release-note}}

Konfigurieren Sie dieses Ziel, um Zielgruppen aus Ihrem Projekt für Adobe Experience Platform zu aktivieren. Durch die Aktivierung von Zielgruppen in Adobe Experience Platform können Sie die Funktionen der Plattform für die Zielgruppensegmentierung, -analyse und -aktivierung über verschiedene Marketing-Kanäle hinweg nutzen. Weitere Informationen zu Adobe Experience Platform finden Sie in der [Übersicht über Experience Platform](https://experienceleague.adobe.com/de/docs/experience-platform/landing/home){target="_blank"}.

>[!NOTE]
>
>Derzeit können nur Herausgeber Ziele in Real-Time CDP Collaboration konfigurieren.

## Konfigurieren des Ziels {#configure-destination}

Um Adobe Experience Platform als Ziel zu konfigurieren, navigieren Sie zu **[!UICONTROL Setup]** und wählen Sie dann die Registerkarte **[!UICONTROL Ziele]** aus. Wählen Sie **[!UICONTROL Einrichten]** für Adobe Experience Platform aus.

![Der Arbeitsbereich „Meine Ziele“ mit der hervorgehobenen Option „Einrichten“ für das Adobe Experience Platform-Ziel.](/help/assets/destinations/adobe-experience-platform/setup-aep.png)

Der **[!UICONTROL Ziel erstellen]** wird angezeigt.

![Der Ziel-Workflow für Adobe Experience Platform erstellen.](/help/assets/destinations/adobe-experience-platform/create-destination.png)

### Sandbox konfigurieren {#configure-sandbox}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_audience_expiration"
>title="Zielgruppen-Gültigkeit"
>abstract="Der Zeitraum, nach dem die Zielgruppe in Adobe Experience Platform nicht mehr verfügbar sein wird. Die Standardgültigkeit beträgt 30 Tage, Sie können sie jedoch auf einen beliebigen Wert zwischen 1 und 30 Tagen festlegen."

Zunächst müssen Sie die Sandbox auswählen, an die Ihre Zielgruppendaten gesendet werden.

>
>
>Sie können nur eine Sandbox auswählen, auf die Ihre Benutzerin oder Ihr Benutzer Zugriff hat. Standardmäßig haben alle Real-Time CDP Collaboration-Benutzer Zugriff auf die **Prod**-Sandbox. Um Zugriff auf zusätzliche Sandboxes zu erhalten, muss ein Administrator zusätzliche Sandboxes zu einer Rolle hinzufügen, die Ihrem Benutzer zugewiesen ist. Weitere Informationen zur Verwaltung von Rollen finden Sie im [Rollen verwalten](../permissions/manage-roles.md).

Wählen **[!UICONTROL Abschnitt Sandbox konfigurieren]** die Dropdown-Liste **[!UICONTROL Sandbox]** aus oder geben Sie den Namen einer Sandbox ein.

![Das hervorgehobene Dropdown-Menü „Sandbox“ im Workflow „Ziel erstellen“.](/help/assets/destinations/adobe-experience-platform/select-sandbox.png)

Alternativ können Sie auf **[!UICONTROL Sandbox durchsuchen]** klicken, um alle verfügbaren Sandboxes sowie deren **[!UICONTROL Typ]**, **[!UICONTROL Status]** und **[!UICONTROL Region]** anzuzeigen. Wählen Sie die zu verwendende Sandbox und dann **[!UICONTROL Speichern]** aus.

Konfigurieren Sie anschließend die **[!UICONTROL Zielgruppengültigkeit]**. Standardmäßig ist der Ablauf der Zielgruppe auf 30 Tage festgelegt. Sie können die Gültigkeit zwischen 1 und 30 Tagen festlegen. Nach dem Ablaufdatum ist die Zielgruppe in Adobe Experience Platform nicht mehr verfügbar.

![Der Abschnitt zur Gültigkeit der Zielgruppe, der im Workflow zum Erstellen eines Ziels hervorgehoben ist.](/help/assets/destinations/adobe-experience-platform/audience-expiration.png)

### Aktivierungs-Zuordnung erstellen {#create-activation-mapping}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_activation_matchkeys"
>title="Aktivierungs-Übereinstimmungsschlüssel"
>abstract="Übereinstimmungsschlüssel für die Aktivierung werden basierend auf den Übereinstimmungsschlüsseln angezeigt, die Sie beim Erstellen Ihrer Organisation ausgewählt haben."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="Zielgruppen-Namespaces"
>abstract="Ziel-Namespaces geben an, welchem Identity-Namespace der Übereinstimmungsschlüssel in Adobe Experience Platform zugeordnet wird. Hash-Übereinstimmungsschlüssel müssen einem Ziel-Namespace zugeordnet werden, der Hash-Werte unterstützt."

Als Nächstes müssen Sie ein Aktivierungszuordnung erstellen, um zu definieren, wie die Zielgruppendaten an Adobe Experience Platform gesendet werden. Sie können jeden [Übereinstimmungsschlüssel](../setup/onboard-organization.md#set-up-match-keys) den Sie beim Erstellen Ihrer Organisation ausgewählt haben, einem Ziel-Namespace zuordnen. Die Ziel-Namespaces geben an[ welchem ](https://experienceleague.adobe.com/de/docs/experience-platform/identity/features/namespaces#standard){target="_blank"}Identitäts-Namespace) der Übereinstimmungsschlüssel in Adobe Experience Platform zugeordnet wird.

>
>
>Hash-Übereinstimmungsschlüssel müssen einem Ziel-Namespace zugeordnet werden, der Hash-Werte unterstützt. Beispielsweise muss der Übereinstimmungsschlüssel **[!UICONTROL gehashte E-Mail]** dem Identity-Namespace **[!UICONTROL E-Mail(SHA256, in Kleinbuchstaben)]** in Adobe Experience Platform zugeordnet werden. Der Übereinstimmungsschlüssel **[!UICONTROL gehashte E-Mail]** kann nicht dem Identity-Namespace **[!UICONTROL E-Mail]** zugeordnet werden, da dieser Namespace keine Hash-Werte unterstützt.

Wählen Sie **[!UICONTROL Feld]** Target-Namespaces“ neben jedem Übereinstimmungsschlüssel. Das **[!UICONTROL Quellfeld auswählen]** wird angezeigt. Suchen Sie den Ziel-Namespace in der Liste oder suchen Sie nach einem bestimmten Namespace. Wählen Sie den Ziel-Namespace aus, den Sie für den Übereinstimmungsschlüssel verwenden möchten, und wählen Sie dann **[!UICONTROL Auswählen]** aus.

![Das Dialogfeld „Quellfeld auswählen“ mit hervorgehobener Option „Auswählen“..](/help/assets/destinations/adobe-experience-platform/select-target-namespace.png)

Wenn Sie die Zuordnung aller Übereinstimmungsschlüssel abgeschlossen haben, überprüfen Sie Ihre Einstellungen und wählen Sie dann **[!UICONTROL Erstellen]** aus, um die Erstellung Ihres Ziels abzuschließen.

## Verwenden von Adobe Experience Platform als Ziel

Nachdem Sie Adobe Experience Platform als Ziel konfiguriert haben, können Sie mit dem [Aktivieren von Zielgruppen](../collaborate/activate.md) über Ihre Projekte beginnen. Derzeit ist der Aktivierungsprozess ein einstufiger Prozess, der vom Advertiser initiiert wird. Wenn der Advertiser eine Zielgruppe aktiviert, wird sie an das vorkonfigurierte Ziel des Publishers (in diesem Fall Adobe Experience Platform) gesendet. Der Herausgeber muss keine zusätzlichen Schritte ausführen, um die Zielgruppe an das Ziel zu senden.

>[!IMPORTANT]
>
>Sie **müssen** Adobe Experience Platform als Ziel konfigurieren *bevor* Mitarbeiter eine Zielgruppe aktiviert. Wenn das Ziel nicht konfiguriert ist, wird die Zielgruppe an Sie gesendet und auf der Registerkarte **[!UICONTROL Aktivieren]** innerhalb eines Projekts angezeigt, sie wird jedoch nicht für Adobe Experience Platform aktiviert.

Experience Platform Nachdem die Zielgruppe aktiviert wurde, ist sie im [Zielgruppenportal) in ](#audience-portal) mit Real-Time CDP Collaboration als Ursprung verfügbar.  Diese Zielgruppen können dann in Kampagnen und in der Kundeninteraktion verwendet werden.

### Zielgruppen-Portal {#audience-portal}

Nachdem Sie Adobe Experience Platform als Ziel konfiguriert haben, können Sie die aktivierten Zielgruppen im Zielgruppenportal anzeigen. Audience Portal ist ein zentraler Knotenpunkt in Adobe Experience Platform, über den Sie Ihre Zielgruppen anzeigen und verwalten können. Zielgruppenportal bietet jetzt Real-Time CDP Collaboration als Herkunft beim Filtern Ihrer Zielgruppen.

>[!IMPORTANT]
>
>Sie sind dafür verantwortlich, alle erforderlichen Datennutzungskennzeichnungen auf die Zielgruppen anzuwenden, die Sie für Adobe Experience Platform aktivieren. Weitere Informationen finden Sie im Handbuch [Datennutzungskennzeichnungen](https://experienceleague.adobe.com/de/docs/experience-platform/data-governance/labels/overview){target="_blank"} .

![Das Zielgruppenportal mit Real-Time CDP Collaboration als Ursprung in den Filteroptionen.](/help/assets/destinations/adobe-experience-platform/audience-portal.png)

Weitere Informationen zu Audience Portal finden Sie im Handbuch [Audience Portal - Übersicht](https://experienceleague.adobe.com/de/docs/experience-platform/segmentation/ui/audience-portal#manage-audiences){target="_blank"} .
