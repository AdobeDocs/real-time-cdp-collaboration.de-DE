---
title: Erstellen und Verwalten von Projekten
description: Erfahren Sie, wie Sie in Adobe Real-Time CDP Collaboration Projekte erstellen und verwalten
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: ae492846-bc0a-4422-86ca-577bcc1fa60c
source-git-commit: 0cf888e36ffc4730fc8de4d8adccae0e0fc2caa8
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 11%

---

# Erstellen und Verwalten von Projekten

{{limited-availability-release-note}}

Projekte sind das Herzstück Ihres Workflows in Adobe Real-Time CDP Collaboration. Erstellen Sie nach der Verbindung mit Mitarbeitern ein Projekt, um Berechnungen der Zielgruppenüberschneidung durchzuführen und relevante Zielgruppen für Kampagnen zu ermitteln.

>[!TIP]
>
>Projekte sollten im Allgemeinen mit einer einzelnen Kampagne verknüpft werden.

![Das Dashboard „Zusammenarbeit“ zeigt alle aktuellen Projekte an.](/help/assets/collaborate/manage-view-projects/projects-overview-page.png){zoomable="yes"}

Sie können Filter verwenden, um nur die Projekte anzuzeigen, die Sie mit bestimmten Partnern begonnen haben, wie unten dargestellt:

![Gefilterte Ansicht von Projekten mit einem einzelnen Mitarbeiter.](/help/assets/collaborate/manage-view-projects/filtered-project-view.png){zoomable="yes"}

## Erstellen eines Projekts {#create-project}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_create_project_advertisername_amc"
>title="Advertiser-Name (Amazon Marketing Cloud)"
>abstract="Bei Amazon Marketing Cloud-Verbindungen (AMC) stellt dieses Feld die AMC-Instanz dar, auf die Ihr Amazon Ads-Login Zugriff hat. Es gibt keinen Advertiser-Namen an. Falls die erforderliche Instanz nicht aufgeführt ist, wenden Sie sich an Ihre bzw. Ihren Amazon Marketing Cloud-Admin, um Zugriff anzufordern."

Um ein Projekt zu erstellen, müssen Sie zunächst [Verbindung herstellen](/help/guide/connect/establishing-connections.md) mit einem Mitarbeiter herstellen. Sobald die Verbindung hergestellt ist, können Sie mit diesem Partner ein Projekt erstellen.

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_projects_advertisername"
>title="Advertiser-Name"
>abstract="Wählen Sie den Advertiser-Namen aus dem Dropdown-Menü aus. Die Optionen werden vom Publisher in den Verbindungseinstellungen vorkonfiguriert, um die Kompatibilität mit den Systemen sicherzustellen."

Navigieren Sie zu **[!UICONTROL Zusammenarbeiten]** und dann **[!UICONTROL Meine Projekte]**. Wenn dies Ihr erstes Projekt ist, können Sie **[!UICONTROL Projekt erstellen]** auswählen. Andernfalls können Sie das Symbol zum Hinzufügen auswählen (![Symbol hinzufügen.](/help/assets/icons/plus.png)) um jederzeit ein neues Projekt zu erstellen.

![Wählen Sie ein Pluszeichen oder Erstellen Sie ein Projekt, um ein neues Projekt einzurichten.](/help/assets/collaborate/manage-view-projects/create-project.png){zoomable="yes"}

Das **[!UICONTROL Projekt erstellen]** wird angezeigt. Wählen Sie **[!UICONTROL Dropdown]** Menü aus, mit dem Sie das Projekt erstellen möchten. Wenn Sie Publisher sind und bei der Einrichtung Ihrer Verbindung Advertiser-Namen festlegen, können Sie den **[!UICONTROL Advertiser-Name]** auswählen.

>[!NOTE]
>
> Wenn Sie in den Verbindungseinstellungen einen einzelnen Advertiser-Namen konfiguriert haben, wird er standardmäßig angezeigt. Wenn kein Werbekunden-Name eingerichtet wurde, wird der **[!UICONTROL Name]** des Werbekunden als **[!UICONTROL Werbekunden-Name]** vorausgewählt.

![Dialogfeld „Projekt erstellen“ mit ausgewähltem Mitarbeiter und hervorgehobenem Advertiser-Namen.](/help/assets/collaborate/manage-view-projects/create-project-advertiser-names.png){zoomable="yes"}

Fügen Sie anschließend einen **[!UICONTROL Projektnamen]** und **[!UICONTROL Beschreibung]** für Ihr Projekt hinzu. Wählen Sie dann ein Bild für das Projekt aus. Dieses Bild hilft, das Projekt auf der Seite „Projektübersicht“ zu unterscheiden. Wenn Sie fertig sind, wählen Sie **[!UICONTROL Erstellen]** aus, um das Projekt zu erstellen.

![Erforderliche Optionen zum Einrichten eines neuen Projekts](/help/assets/collaborate/manage-view-projects/create-project-required-info.png){zoomable="yes"}

Jetzt können Sie Ihr neues Projekt, seine Details und verfügbaren Abschnitte basierend auf den Anwendungsfällen anzeigen, die bei der Einrichtung der Verbindung ausgewählt wurden.

![Der Arbeitsbereich „Projektübersicht“.](/help/assets/collaborate/manage-view-projects/project-overview.png){zoomable="yes"}

## Kampagnen-ID verwalten {#manage-campaign-id}

Eine **Kampagnen-ID** verknüpft Ihr Projekt mit einer bestimmten Kampagne und ist erforderlich, um [Messberichte zu generieren](./measure.md#create-measurement-report). Sie können einem Projekt mehrere Kampagnen-IDs hinzufügen, wenn Sie mehrere Kampagnen mit demselben Mitarbeiter ausführen. Alle diese Kampagnen stehen im Reporting zur Auswahl.

- **Herausgeber**: Geben Sie Kampagnen-IDs und zugehörige Namen in die Collaboration-Benutzeroberfläche ein oder aktualisieren Sie sie, bevor Sie Berichte ausführen.
- **Advertisers**: Bitten Sie Ihren Mitarbeiter (Publisher), bei Bedarf Kampagnen-IDs hinzuzufügen.

Um Kampagnen-IDs hinzuzufügen oder zu aktualisieren, navigieren Sie zum Arbeitsbereich **[!UICONTROL Zusammenarbeiten]** und wählen Sie dann **[!UICONTROL Anzeigen]** in der entsprechenden Projektkarte aus.

![Der Arbeitsbereich „Zusammenarbeiten“, in dem die Option „Anzeigen“ auf einer Projektkarte hervorgehoben ist.](/help/assets/collaborate/manage-view-projects/view-project.png){zoomable="yes"}

Der entsprechende Arbeitsbereich **[!UICONTROL Projektübersicht]** wird mit einem Abschnitt **[!UICONTROL Kampagnen-ID und -Name]** angezeigt, in dem alle mit dem Projekt verknüpften Kampagnen aufgeführt sind. Wenn Sie noch keine Kampagne hinzugefügt haben, wählen Sie **[!UICONTROL Hinzufügen]** aus. Wenn bereits Kampagnen vorhanden sind, wählen Sie **[!UICONTROL Bearbeiten]** aus, um die Details zu aktualisieren oder zusätzliche hinzuzufügen.

![Der Arbeitsbereich „Projektübersicht“, in dem der Abschnitt „Kampagnen-ID und -Name“ mit der hervorgehobenen Option „Bearbeiten“ angezeigt wird.](/help/assets/collaborate/manage-view-projects/edit-campaign-id.png){zoomable="yes"}

Wählen Sie im Dialogfeld **[!UICONTROL Kampagnen-ID und -Name]** die Option **[!UICONTROL Kampagnen-ID hinzufügen]**, um eine neue Zeile hinzuzufügen, in der Sie Kampagnendetails eingeben können.

![Im Dialogfeld Kampagnen-ID und -Name wird nach Auswahl der Option Kampagnen-ID hinzufügen die leere Kampagnenzeile angezeigt.](/help/assets/collaborate/manage-view-projects/add-campaign-row.png){zoomable="yes"}

Geben Sie die **[!UICONTROL Kampagnen-ID]** und **[!UICONTROL Kampagnenname]** ein und wählen Sie dann **[!UICONTROL Speichern]**.

![Das Dialogfeld für die Kampagnen-ID und den Namen mit hervorgehobenen neuen Kampagnendetails und der hervorgehobenen Option „Speichern“.](/help/assets/collaborate/manage-view-projects/save-campaign-id.png){zoomable="yes"}

Im Abschnitt **[!UICONTROL Kampagnenkennung und -name]** finden Sie Ihre neuesten Kampagnen und Änderungen. Sie können jetzt die neuen Kampagnen-IDs verwenden, um Messberichte zu generieren.

![Der Arbeitsbereich Projektübersicht mit dem aktualisierten Abschnitt Kampagnen-ID und -Name.](/help/assets/collaborate/manage-view-projects/view-updated-campaigns.png){zoomable="yes"}
