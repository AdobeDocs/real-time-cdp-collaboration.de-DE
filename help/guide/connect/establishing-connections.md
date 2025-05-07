---
title: Verbinden mit Werbetreibenden oder Herausgebern
description: Erfahren Sie, wie Sie nach der Entdeckung potenzieller Mitarbeiter Verbindungen herstellen und Projekte gemeinsam bearbeiten können.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: e0894fb3cb290334e0e95d5c26288705967d9dbe
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 13%

---

# Verbinden mit Werbetreibenden oder Herausgebern

{{limited-availability-release-note}}

Die Herstellung einer Verbindung zwischen zwei Parteien einer Kollaboration (meistens ein Advertiser und ein Publisher) ist die Voraussetzung in Real-Time CDP Collaboration für Unternehmen, die an Kampagnen zusammenarbeiten. Sowohl Publisher als auch Advertiser können Verbindungen einrichten. Der Teilnehmer, der die Verbindung herstellt, ist anschließend der *Verbindungseigentümer*.

## Workflow auf hoher Ebene

Um eine Verbindung zwischen einem Advertiser und einem Publisher herzustellen, sieht der Workflow auf allgemeiner Ebene wie folgt aus:

1. Der Werbetreibende [durchsucht Verlage und entdeckt](/help/guide/connect/discover-publishers.md) einen, mit dem er arbeiten möchte
2. Der Advertiser sendet eine Einladung zur Verbindung.
3. Der Herausgeber nimmt die Einladung an.
4. Der Advertiser sendet Verbindungseinstellungen einschließlich Übereinstimmungsschlüsseln und anderen. Diese Verbindungseinstellungen stellen die produktinternen Bedingungen der Zusammenarbeit dar.
5. Der Publisher akzeptiert Verbindungseinstellungen. Falls gewünscht, kann der Publisher die anfänglichen Verbindungseinstellungen ablehnen und den Advertiser auffordern, geänderte Verbindungseinstellungen zu übermitteln.

![Allgemeine Abbildung des Verbindungsprozesses zwischen Advertiser und Publisher.](/help/assets/connect/establish-connection/advertiser-publisher-connection-process.png){zoomable="yes"}

Sobald die oben genannten Elemente abgeschlossen sind, können die Mitwirkenden mit dem [Erstellen eines Projekts](/help/guide/collaborate/manage-projects.md#create-project) fortfahren, [Überschneidungsberichte auszuführen](/help/guide/collaborate/discover.md) und Werbekampagnen zu starten.

>[!IMPORTANT]
>
>Nachdem die Verbindung zwischen zwei Partnern hergestellt wurde, können die Verbindungseinstellungen nicht mehr geändert werden.

## Einladung senden {#send-invite}

Um eine Verbindung einzurichten, wählen Sie **[!UICONTROL Verbinden]** beim Durchsuchen des Publisher-Inventars im Bildschirm „Publisher erkennen“ aus.

![Verbindungsauswahl](/help/assets/connect/establish-connection/connect-selection.png){zoomable="yes"}

An dieser Stelle ist die Einladung deaktiviert und Sie können die Verbindungseinstellungen in der Vorschau anzeigen, sie jedoch nicht bearbeiten. Sie können die ausstehende Einladung auf der Registerkarte **[!UICONTROL Meine Verbindungen]** anzeigen. Der Status der Verbindung lautet &quot;**[!UICONTROL gesendet]**.

![Ausstehende Einladung an Herausgeber gesendet, in der Ansicht „Meine Verbindungen“ angezeigt.](/help/assets/connect/establish-connection/pending-invite-sent.png){zoomable="yes"}

Sobald der Mitarbeiter die Einladung akzeptiert, können Sie die Verbindungseinstellungen konfigurieren und an den Mitarbeiter senden, um sie zu überprüfen und zu akzeptieren.

## Verbindungseinstellungen {#connection-settings}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_usecases"
>title="Anwendungsfälle"
>abstract="Die Anwendungsszenarien sind mit allen Optionen vorausgefüllt. Sie können die Anwendungsszenarien bearbeiten, bevor Sie Ihre Verbindungseinstellungen übermitteln."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_matchkeys"
>title="Übereinstimmungsschlüssel"
>abstract="Übereinstimmungsschlüssel werden mit den Schlüsseln vorausgefüllt, die Sie auf Organisationsebene ausgewählt haben. Sie können alle Übereinstimmungsschlüssel deaktivieren, die Sie in dieser Verbindung nicht verwenden möchten."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit"
>title="Credit-Aufspaltung"
>abstract="In diesem Abschnitt wird festgelegt, wer die Kosten für die entsprechenden Aktivitäten in Real-Time CDP Collaboration trägt. Derzeit ist nur der Anwendungsfall für die Freigabe von Zielgruppen konfigurierbar."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="Freigabe von Zielgruppen"
>abstract="Die Freigabe von Zielgruppen ist die Aktivität, die eine Partei ausführt, wenn sie die Aktivierung ihrer abgeglichenen Daten durch ihren Kooperationspartner anfordert."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_measurement"
>title="Messung"
>abstract="In diesem Anwendungsbeispiel können Sie Aktivitäten in Real-Time CDP Collaboration ausführen, um Leistungsberichte und Einblicke für Kampagnen zu generieren."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_legalagreement"
>title="Rechtlicher Vertrag"
>abstract="Stellen Sie sicher, dass ein Vertrag über die Datenfreigabe zwischen den beiden Parteien besteht."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_advertisername"
>title="Advertiser-Namen"
>abstract="Gibt die Aliase an, unter denen der Advertiser dem Publisher bekannt ist. "

Nachdem die Einladung gesendet wurde, können Sie eine Vorschau der Verbindungseinstellungen anzeigen. Die Einladung muss angenommen werden, bevor Sie die Einrichtung der Verbindung abschließen können.

![Die Ansicht mit den Verbindungseinstellungen im Vorschaustatus.](/help/assets/connect/establish-connection/preview-connection-settings.png){zoomable="yes"}

Sobald die Verbindung von Ihrem Mitarbeiter akzeptiert wurde, können Sie mit dem Einrichten der Verbindungseinstellungen für die Verbindung beginnen. Die Verbindungseinstellungen definieren die Bedingungen für Ihre Zusammenarbeit, z. B. die Anwendungsfälle, die Sie gemeinsam ausführen, die Übereinstimmungsschlüssel, die Sie in Projekten verwenden werden, und mehr.

Um Verbindungseinstellungen für Ihren Mitarbeiter einzurichten und freizugeben, navigieren Sie zu **[!UICONTROL Meine Verbindungen]**. Für alle Verbindungen mit dem Status **[!UICONTROL Ausstehend]** können Sie **[!UICONTROL Verbindung einrichten]** auswählen, um die Verbindungseinstellungen zu konfigurieren.

![Die Ansicht „Meine Verbindungen“ mit einer hervorgehobenen Option „Ausstehende Verbindung“ und „Verbindung einrichten“.](/help/assets/connect/establish-connection/pending-connection.png){zoomable="yes"}

Sie können die folgenden Felder bearbeiten und definieren:

![Einrichten der Verbindungsansicht](/help/assets/connect/establish-connection/connection-view.png){zoomable="yes"}

+++Anwendungsfälle

Anwendungsfälle sind mit allen verfügbaren Anwendungsfällen vorausgefüllt. Sie können auswählen, welche Anwendungsfälle Ihre Verbindung verwenden soll, indem Sie **[!UICONTROL Bearbeiten]** auswählen und alle Anwendungsfälle deaktivieren, die Sie nicht möchten. Ausgewählte Anwendungsfälle wirken sich darauf aus, welche Ansichten und Optionen in [ Projekten verfügbar ](../collaborate/manage-projects.md#project-use-cases).

![Anwendungsbeispiele](/help/assets/connect/establish-connection/view-use-cases.png){zoomable="yes"}

+++

+++Übereinstimmungsschlüssel

Übereinstimmungsschlüssel werden mit den Schlüsseln vorbefüllt, die Sie [auf Organisationsebene ausgewählt](/help/guide/setup/onboard-organization.md#set-up-match-keys). Sie können alle Übereinstimmungsschlüssel deaktivieren, die in dieser Verbindung nicht verwendet werden sollen. Sie können jedoch keine Übereinstimmungsschlüssel hinzufügen, die beim Einrichten der Organisation nicht ausgewählt wurden.

![Übereinstimmungsschlüssel](/help/assets/connect/establish-connection/match-keys.png)

+++

+++Kreditaufteilung

Verwenden Sie den Abschnitt „Kreditaufteilung“, um zu bestimmen, welche der beiden kooperierenden Parteien die Kosten für die Aktivitäten deckt.

![Kreditaufteilung](/help/assets/connect/establish-connection/edit-billing-ownership.png)

+++

+++Vereinbarungen

Bevor Sie mit dieser Verbindung fortfahren können, müssen Sie anerkennen, dass eine Datenfreigabevereinbarung zwischen den beiden Parteien besteht.

![Rechtliche Vereinbarungen.](/help/assets/connect/establish-connection/legal-agreement.png)

+++

Nachdem Sie Ihre Auswahl getroffen haben, klicken Sie auf **[!UICONTROL Senden]**, um die vorgeschlagenen Einstellungen zur Überprüfung an Ihren Mitarbeiter zu senden.

Wenn Sie vorgeschlagene Verbindungseinstellungen von Ihrem Mitarbeiter erhalten, können Sie diese Einstellungen entweder **[!UICONTROL Akzeptieren]** oder **[!UICONTROL Ablehnen]**. Bevor Sie die Verbindungseinstellungen akzeptieren, müssen Sie bestätigen und bestätigen, dass eine rechtliche Vereinbarung zwischen Ihnen und dem Mitarbeiter besteht. Wenn Sie Verbindungseinstellungen ablehnen, wenden Sie sich an einen Mitarbeiter außerhalb des Produkts und besprechen Sie, wie die Verbindungseinstellungen überarbeitet werden sollten, damit Sie sie akzeptieren können.

## Verbindungen löschen {#delete-connections}

Sie können alle Verbindungen mit Partnern löschen, mit denen Sie nicht weiter arbeiten möchten. So löschen Sie bestehende Verbindungen:

1. Navigieren Sie zu **[!UICONTROL Verbinden]** > **[!UICONTROL Meine Verbindungen]**.
2. Wählen **[!UICONTROL auf der]** „Verbindung anzeigen“ aus, um auf die zu löschende Verbindung zuzugreifen.
3. Wählen Sie das Löschsymbol ![Löschsymbol](/help/assets/common/delete.svg), um das Bestätigungsdialogfeld für das Löschen der Verbindung aufzurufen.
   ![Symbol „Verbindung löschen“ hervorgehoben.](/help/assets/connect/establish-connection/delete-icon-highlighted.png){zoomable="yes"}
4. Bestätigen Sie den Löschvorgang, indem Sie **[!UICONTROL Löschen]** auswählen.
   ![Dialogfeld zum Bestätigen des Löschens einer Verbindung. ](/help/assets/connect/establish-connection/delete-connection-dialog.png){zoomable="yes"}

>[!WARNING]
>
>Nachdem die Verbindung gelöscht wurde, sind Sie nicht mehr mit dem Mitarbeiter verbunden und alle vorhandenen Projekte, die Teil der Zusammenarbeit sind, werden dauerhaft gelöscht und können nicht wiederhergestellt werden.

## Nächste Schritte

Nachdem Sie eine Verbindung mit Ihrem Mitarbeiter hergestellt haben, können Sie und Ihr Mitarbeiter jetzt [Projekte erstellen](/help/guide/collaborate/manage-projects.md#create-project).
