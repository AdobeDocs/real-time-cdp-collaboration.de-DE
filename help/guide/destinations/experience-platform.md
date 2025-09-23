---
title: Konfigurieren von Adobe Experience Platform als Ziel
description: Erfahren Sie, wie Sie Adobe Experience Platform as a -Ziel in Real-Time CDP Collaboration konfigurieren und verwalten.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 594610a0-9102-448a-b59b-ec162ef9dd57
source-git-commit: 6acf936f50b412147578a70e2369b06c53260f06
workflow-type: tm+mt
source-wordcount: '1487'
ht-degree: 11%

---

# Konfigurieren von Adobe Experience Platform als Ziel

{{limited-availability-release-note}}

Konfigurieren Sie dieses Ziel, um Zielgruppen aus Ihrem Projekt für Adobe Experience Platform zu aktivieren. Durch die Aktivierung von Zielgruppen in Adobe Experience Platform können Sie die Funktionen der Plattform für die Zielgruppensegmentierung, -analyse und -aktivierung über verschiedene Marketing-Kanäle hinweg nutzen. Weitere Informationen zu Adobe Experience Platform finden Sie in der [Übersicht über Experience Platform](https://experienceleague.adobe.com/de/docs/experience-platform/landing/home){target="_blank"}.

>[!WARNING]
>
>Sie können ein Ziel nicht aktualisieren, nachdem es erstellt wurde. Wenn Sie Einstellungen ändern müssen, müssen Sie das vorhandene Ziel löschen und ein neues erstellen.

## Konfigurieren des Ziels {#configure-destination}

Um Adobe Experience Platform als Ziel zu konfigurieren, gehen Sie zu **[!UICONTROL Setup]** und wählen Sie dann die Registerkarte **[!UICONTROL Meine Ziele]** aus. Wählen Sie **[!UICONTROL Einrichten]** für Adobe Experience Platform aus.

![Der Arbeitsbereich „Meine Ziele“ mit der hervorgehobenen Option „Einrichten“ für das Adobe Experience Platform-Ziel.](/help/assets/destinations/adobe-experience-platform/setup-aep.png)

Der **[!UICONTROL Ziel erstellen]** wird angezeigt.

![Der Ziel-Workflow für Adobe Experience Platform erstellen.](/help/assets/destinations/adobe-experience-platform/create-destination.png)

### Konfigurieren einer Sandbox {#configure-sandbox}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_audience_expiration"
>title="Zielgruppen-Gültigkeit"
>abstract="Der Zeitraum, nach dem die Zielgruppe in Adobe Experience Platform nicht mehr verfügbar ist. Die Standardgültigkeit beträgt 30 Tage, Sie kann jedoch auf einen beliebigen Wert zwischen 1 und 30 Tagen festgelegt werden."

Zunächst müssen Sie die Sandbox auswählen, an die Ihre Zielgruppendaten gesendet werden.

>[!IMPORTANT]
>
>Sie können nur eine Sandbox auswählen, auf die Ihre Benutzerin oder Ihr Benutzer Zugriff hat. Standardmäßig haben alle Collaboration-Benutzer Zugriff auf die **Prod**-Sandbox. Um Zugriff auf zusätzliche Sandboxes zu erhalten, muss ein Administrator zusätzliche Sandboxes zu einer Rolle hinzufügen, die Ihrem Benutzer zugewiesen ist. Weitere Informationen zur Verwaltung von Rollen finden Sie im [Rollen verwalten](../permissions/manage-roles.md).

Wählen **[!UICONTROL Abschnitt Sandbox konfigurieren]** die Dropdown-Liste **[!UICONTROL Sandbox]** aus oder geben Sie den Namen einer Sandbox ein.

![Das hervorgehobene Dropdown-Menü „Sandbox“ im Workflow „Ziel erstellen“.](/help/assets/destinations/adobe-experience-platform/select-sandbox.png)

Alternativ können Sie auf **[!UICONTROL Sandbox durchsuchen]** klicken, um alle verfügbaren Sandboxes sowie deren **[!UICONTROL Typ]**, **[!UICONTROL Status]** und **[!UICONTROL Region]** anzuzeigen. Wählen Sie die zu verwendende Sandbox und dann **[!UICONTROL Speichern]** aus.

Konfigurieren Sie anschließend die **[!UICONTROL Zielgruppengültigkeit]**. Standardmäßig ist der Ablauf der Zielgruppe auf 30 Tage festgelegt. Sie können die Gültigkeit zwischen 1 und 30 Tagen festlegen. Nach dem Ablaufdatum ist die Zielgruppe in Adobe Experience Platform nicht mehr verfügbar.

![Der Abschnitt zur Gültigkeit der Zielgruppe, der im Workflow zum Erstellen eines Ziels hervorgehoben ist.](/help/assets/destinations/adobe-experience-platform/audience-expiration.png)

### Erstellen einer Aktivierungszuordnung {#create-activation-mapping}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_activation_matchkeys"
>title="Aktivierungs-Übereinstimmungsschlüssel"
>abstract="Übereinstimmungsschlüssel für die Aktivierung werden basierend auf den Übereinstimmungsschlüsseln angezeigt, die beim Erstellen der Organisation ausgewählt wurden."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="Ziel-Namespaces"
>abstract="Zielgruppen-Namespaces geben an, welchem Identity-Namespace der Übereinstimmungsschlüssel in Adobe Experience Platform zugeordnet wird. Hash-Übereinstimmungsschlüssel müssen einem Zielgruppen-Namespace zugeordnet sein, der Hash-Werte unterstützt."

Alle für Ihr Konto aktivierten Übereinstimmungsschlüssel sind standardmäßig in der Aktivierungszuordnung enthalten. Wenn Sie einen Übereinstimmungsschlüssel nicht direkt einem Ziel-Namespace zuordnen möchten, können Sie die Option Verknüpfter Schlüssel verwenden, um ihn durch einen anderen Übereinstimmungsschlüssel zu ersetzen. Weitere Informationen zu verknüpften Schlüsseln finden Sie [ Abschnitt unten](#linked-keys).

#### Zuordnen von Ziel-Namespaces {#map-target-namespaces}

Um jeden Übereinstimmungsschlüssel einem Ziel-Namespace zuzuordnen, wählen Sie das Feld **[!UICONTROL Target-]**) neben dem Übereinstimmungsschlüssel aus. Das **[!UICONTROL Quellfeld auswählen]** wird angezeigt. Suchen Sie den Ziel-Namespace in der Liste oder suchen Sie nach einem bestimmten Namespace. Wählen Sie den Ziel-Namespace aus, den Sie für den Übereinstimmungsschlüssel verwenden möchten, und wählen Sie dann **[!UICONTROL Auswählen]** aus.

>[!IMPORTANT]
>
>Hash-Übereinstimmungsschlüssel müssen einem Ziel-Namespace zugeordnet werden, der Hash-Werte unterstützt. Beispielsweise muss der Übereinstimmungsschlüssel **[!UICONTROL gehashte E-Mail]** dem Identity-Namespace **[!UICONTROL E-Mail(SHA256, in Kleinbuchstaben)]** in Adobe Experience Platform zugeordnet werden. Der Übereinstimmungsschlüssel **[!UICONTROL gehashte E-Mail]** kann nicht dem Identity-Namespace **[!UICONTROL E-Mail]** zugeordnet werden, da dieser Namespace keine Hash-Werte unterstützt.

![Das Dialogfeld „Quellfeld auswählen“ mit hervorgehobener Option „Auswählen“..](/help/assets/destinations/adobe-experience-platform/select-target-namespace.png)

Wiederholen Sie diesen Vorgang für jeden Übereinstimmungsschlüssel, den Sie in die Aktivierungszuordnung aufnehmen möchten. Wenn Sie keinen Übereinstimmungsschlüssel einbeziehen möchten, können Sie ihn entfernen oder die Option Verknüpfter Schlüssel verwenden, um ihn durch einen anderen Übereinstimmungsschlüssel zu ersetzen.

#### Verknüpfte Schlüssel {#linked-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_linked_key"
>title="Verknüpfter Schlüssel"
>abstract="Mithilfe verknüpfter Schlüssel können Sie festlegen, dass bei der Aktivierung anstelle des ursprünglichen Übereinstimmungsschlüssels ein anderer Übereinstimmungsschlüssel verwendet werden soll. Damit ein Profil aktiviert wird, muss es Werte sowohl für den ursprünglichen Übereinstimmungsschlüssel als auch für den verknüpften Übereinstimmungsschlüssel aufweisen."

Mithilfe verknüpfter Schlüssel können Sie festlegen, dass bei der Aktivierung anstelle des ursprünglichen Übereinstimmungsschlüssels ein anderer Übereinstimmungsschlüssel verwendet werden soll. Um besser zu verstehen, wie verknüpfte Schlüssel funktionieren, sehen Sie sich folgendes Beispiel an:

Ein retailer möchte die aktivierten Daten an Experience Platform an sein CRM-System senden. Die retailer hat gehashte IP als Übereinstimmungsschlüssel für ihr Konto aktiviert, um die Übereinstimmungsrate beim Aktivieren von Zielgruppen zu erhöhen. Das CRM-System der retailer unterstützt jedoch keine Hash-IP als Identity-Namespace. Daher sollte stattdessen der Übereinstimmungsschlüssel der CRM-ID beim Aktivieren von Zielgruppen für Experience Platform verwendet werden. Die retailer kann die Option „Verknüpfter Schlüssel“ verwenden, um Zielgruppen für Experience Platform mithilfe der CRM-ID statt der Hash-IP zu aktivieren.

>[!NOTE]
>
>Damit ein Profil aktiviert wird, muss es Werte sowohl für den ursprünglichen Übereinstimmungsschlüssel als auch für den verknüpften Übereinstimmungsschlüssel haben. Wenn beispielsweise die Hash-ID mit der CRM-ID verknüpft ist, muss ein Profil Werte sowohl für die Hash-ID als auch für die CRM-ID haben, um aktiviert zu werden. Wenn einer der Werte fehlt, wird das Profil nicht aktiviert.

Um einen verknüpften Schlüssel zu verwenden, aktivieren Sie die Option **[!UICONTROL Verknüpfter Schlüssel]** neben dem Übereinstimmungsschlüssel, den Sie an seiner Stelle verwenden möchten. Der Abschnitt **[!UICONTROL Verknüpfter Schlüssel]** wird angezeigt und Sie werden aufgefordert, die Zuordnung zu erstellen.

![Die Option und der Abschnitt „Verknüpfter Schlüssel“, die im Workflow zum Erstellen eines Ziels hervorgehoben sind.](/help/assets/destinations/adobe-experience-platform/linked-key.png)

Wählen Sie im Dropdown **[!UICONTROL Menü die]** Verknüpfte Taste) aus, die Sie verwenden möchten. Im obigen Beispiel würde die retailer **[!UICONTROL CRM-ID]** als verknüpften Schlüssel auswählen.

![Das hervorgehobene Dropdown-Menü „Verknüpfter Schlüssel“ im Workflow „Ziel erstellen“.](/help/assets/destinations/adobe-experience-platform/select-linked-key.png)

Als Nächstes möchten Sie den Ziel-Namespace für den verknüpften Schlüssel angeben, falls noch nicht geschehen. Wenn Sie den Ziel-Namespace für den Übereinstimmungsschlüssel bereits im Abschnitt **[!UICONTROL Aktivierungszuordnung erstellen]** ausgewählt haben, wird dieser automatisch ausgefüllt. Wenn Sie noch keinen Zielnamespace für den verknüpften Schlüssel ausgewählt haben, können Sie dies jetzt tun.

Wählen Sie **[!UICONTROL Feld]** Target-Namespaces“ neben dem verknüpften Schlüssel. Das **[!UICONTROL Quellfeld auswählen]** wird angezeigt. Suchen Sie den Ziel-Namespace in der Liste oder suchen Sie nach einem bestimmten Namespace. Wählen Sie den Ziel-Namespace aus, den Sie für den verknüpften Schlüssel verwenden möchten, und wählen Sie dann **[!UICONTROL Auswählen]**.

![Das Dialogfeld „Quellfeld auswählen“](/help/assets/destinations/adobe-experience-platform/select-linked-key-target-namespace.png)

Der verknüpfte Schlüssel ist jetzt konfiguriert.

>[!NOTE]
>
>Pro Aktivierungszuordnung kann nur ein verknüpfter Schlüssel-Ziel-Namespace verwendet werden. Wenn Sie beispielsweise die Hash-ID mit der CRM-ID verknüpfen, wird durch Aktivieren der Option Verknüpfter Schlüssel für ein anderes Feld diese auch mit der CRM-ID verknüpft.

Wenn Sie alle Übereinstimmungsschlüssel zugeordnet haben, überprüfen Sie Ihre Einstellungen. Der **[!UICONTROL Vorschau]** Abschnitt enthält eine Zusammenfassung Ihrer Konfiguration.

![Der Abschnitt Vorschau im Workflow zum Erstellen eines Ziels.](/help/assets/destinations/adobe-experience-platform/preview.png)

>[!IMPORTANT]
>
>Derzeit wird jeder Übereinstimmungsschlüssel für Experience Platform als separate Zielgruppe aktiviert. Wenn Sie beispielsweise [!UICONTROL gehashte E-Mail] und [!UICONTROL gehashte Telefon] als Übereinstimmungsschlüssel haben, werden bei der Aktivierung einer Zielgruppe in Audience Portal zwei separate Zielgruppen erstellt.

Wenn Sie mit Ihrer Konfiguration zufrieden sind, wählen Sie **[!UICONTROL Ziel erstellen]** aus. Eine Bestätigungsmeldung wird angezeigt, dass das Ziel erfolgreich erstellt wurde.

## Verwenden von Adobe Experience Platform als Ziel

Nachdem Sie Experience Platform als Ziel konfiguriert haben, können Sie mit dem [Aktivieren von Zielgruppen](../collaborate/activate.md) über Ihre Projekte beginnen. Derzeit ist der Aktivierungsprozess ein einstufiger Prozess, der von dem Mitarbeiter initiiert wird. Wenn beispielsweise ein Advertiser eine Zielgruppe aktiviert, wird sie an das vorkonfigurierte Ziel des Publishers (Experience Platform) gesendet. Der Herausgeber muss keine zusätzlichen Schritte ausführen, um die Zielgruppe an das Ziel zu senden. Dasselbe gilt für das Muster der Zusammenarbeit von Marke zu Marke.

>[!IMPORTANT]
>
>Sie **müssen** Experience Platform als Ziel konfigurieren *bevor* Mitarbeiter eine Zielgruppe aktiviert. Wenn das Ziel nicht konfiguriert ist, wird die Zielgruppe an Sie gesendet und auf der Registerkarte **[!UICONTROL Aktivieren]** innerhalb eines Projekts angezeigt, sie wird jedoch nicht für Experience Platform aktiviert.

Experience Platform Nachdem die Zielgruppe aktiviert wurde, ist sie im [Zielgruppenportal) in ](#audience-portal) mit Real-Time CDP Collaboration als Ursprung verfügbar.  Diese Zielgruppen können dann in Kampagnen und in der Kundeninteraktion verwendet werden.

### Zielgruppenportal {#audience-portal}

Nachdem Sie Adobe Experience Platform als Ziel konfiguriert haben, können Sie die aktivierten Zielgruppen im Zielgruppenportal anzeigen. Audience Portal ist ein zentraler Knotenpunkt in Adobe Experience Platform, über den Sie Ihre Zielgruppen anzeigen und verwalten können. Zielgruppenportal bietet jetzt Real-Time CDP Collaboration als Herkunft beim Filtern Ihrer Zielgruppen.

>[!IMPORTANT]
>
>Sie sind dafür verantwortlich, alle erforderlichen Datennutzungskennzeichnungen auf die Zielgruppen anzuwenden, die Sie für Adobe Experience Platform aktivieren. Weitere Informationen finden Sie im Handbuch [Datennutzungskennzeichnungen](https://experienceleague.adobe.com/de/docs/experience-platform/data-governance/labels/overview){target="_blank"} .

![Das Zielgruppenportal mit Real-Time CDP Collaboration als Ursprung in den Filteroptionen.](/help/assets/destinations/adobe-experience-platform/audience-portal.png)

Weitere Informationen zu Audience Portal finden Sie im Handbuch [Audience Portal - Übersicht](https://experienceleague.adobe.com/de/docs/experience-platform/segmentation/ui/audience-portal#manage-audiences){target="_blank"} .
