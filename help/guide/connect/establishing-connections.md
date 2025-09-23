---
title: Herstellen von Verbindungen
description: Erfahren Sie, wie Sie nach der Entdeckung potenzieller Mitarbeiter Verbindungen herstellen und Projekte gemeinsam bearbeiten können.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: 899b6c2a0111ccaebbaf2818772e1d743d6de914
workflow-type: tm+mt
source-wordcount: '3400'
ht-degree: 7%

---

# Herstellen von Verbindungen {#establishing-connections}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_compare_audiences"
>title="Vergleichen von Zielgruppen"
>abstract="Vergleichen Sie Ihre Zielgruppe mit allen Verbrauchern, die Ihre Amazon-Anzeigen erreichen."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_relevant_audiences"
>title="Relevante Zielgruppen"
>abstract="Zielgruppensegmente in Amazon, bei denen Ihre Zielgruppe die größten Überschneidungen aufweist, wobei nur DSP-Impressions berücksichtigt werden (diese Segmente können nur in der DSP angesprochen werden)."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_resolved_ids"
>title="Aufgelöste IDs"
>abstract="Die Anzahl der IDs, die die Identitätsauflösung von Amazon mithilfe Ihrer Zielgruppendaten auflösen konnte."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlapping_ad_exposed_ids"
>title="Überschneidende, für Anzeigen offengelegte IDs"
>abstract="Dies stellt die Anzahl der „aufgelösten IDs“ aus der hochgeladenen Zielgruppe dar, die auch einer Anzeige über Amazon Ads bereitgestellt wurden."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlap_percentage"
>title="Überschneidung %"
>abstract="Der Anteil der „aufgelösten IDs“, die über Amazon Ads einer Anzeige ausgesetzt wurden."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_amazon_breakdown"
>title="Aufschlüsselung nach Amazon-Anzeigenprodukt"
>abstract="Aufschlüsselung der „sich überschneidenden Anzeigen-exponierten IDs“, die entweder von Amazon Ads Sponsored Product und/oder Amazon Ads DSP erreicht wurden."

{{limited-availability-release-note}}

Bevor Mitwirkende an Kampagnen zusammenarbeiten können, müssen sie eine Verbindung herstellen. Diese Verbindung ermöglicht es ihnen, Zielgruppen zu aktivieren, Projekte zu erstellen und Berichte über die Kampagnenleistung zu erstellen.

Verbindungen werden basierend auf Ihrem ausgewählten Kooperationsmuster hergestellt. Collaboration unterstützt zwei wichtige Kooperationsmuster: „Advertiser-to-Publisher“ und „Brand-to-Brand“. Weitere Informationen zu diesen Mustern finden Sie im Handbuch [Anwendungsfälle](/help/guide/overview/use-cases.md) .

Um zu erfahren, wie Sie eine Verbindung herstellen, lesen Sie den folgenden Abschnitt, der Ihrem Kooperationsmuster entspricht:

- [Verbindung zwischen Advertiser und Publisher](#advertiser-to-publisher-connection)
- [Marke-zu-Marke-Verbindung](#brand-to-brand-connection)

## Verbindung zwischen Advertiser und Publisher {#advertiser-to-publisher-connection}

![Allgemeine Abbildung des Verbindungsprozesses zwischen Advertiser und Publisher.](/help/assets/connect/establish-connection/advertiser-publisher-flow.png){zoomable="yes"}

Im Muster von Advertiser zu Publisher erkennt ein Advertiser einen Publisher, mit dem er arbeiten möchte, über den Arbeitsbereich **[!UICONTROL Discover Publishers]** und sendet eine Verbindungseinladung. Der Publisher prüft dann die Einladung und akzeptiert sie, sodass der Advertiser Verbindungseinstellungen vorschlagen kann. Sobald der Herausgeber die Verbindungseinstellungen akzeptiert, wird die Verbindung hergestellt und beide Mitarbeiter können mit der Arbeit an Projekten beginnen.

### Allgemeine Übersicht

Um eine Verbindung zwischen einem Advertiser und einem Publisher herzustellen, sind die folgenden Schritte erforderlich:

1. [Publisher entdecken](#discover-publishers): Der Advertiser identifiziert potenzielle Publisher, mit denen er zusammenarbeiten soll.
1. [Einladung senden](#send-invite): Der Advertiser sendet eine Einladung zur Verbindung an den ausgewählten Publisher.
1. [Einladung annehmen](#accept-invite): Der Herausgeber prüft und akzeptiert die Einladung.
1. [Verbindungseinstellungen konfigurieren](#configure-connection-settings): Der Advertiser konfiguriert die Verbindungseinstellungen und sendet sie zur Überprüfung an den Publisher.
1. [Verbindungseinstellungen bestätigen](#establish-connection): Der Herausgeber prüft die Verbindungseinstellungen und akzeptiert oder lehnt sie ab. Wenn akzeptiert, wird die Verbindung hergestellt. Bei Ablehnung kann der Herausgeber Feedback für Revisionen außerhalb des Produkts geben. Der Werbetreibende kann dann die Einstellungen überarbeiten und zur Überprüfung erneut senden.

Sobald die Verbindungseinstellungen akzeptiert wurden, wird die Verbindung hergestellt und die Mitarbeiter können [ Projekt erstellen](/help/guide/collaborate/manage-projects.md#create-project) um mit der Zusammenarbeit bei Kampagnen zu beginnen.

## Marke-zu-Marke-Verbindung {#brand-to-brand-connection}

![Allgemeine Abbildung des Verbindungsprozesses zwischen Marken.](/help/assets/connect/establish-connection/brand-to-brand-flow.png){zoomable="yes"}

>[!TIP]
>
>Der Begriff **Marke** wird verwendet, um ein Unternehmen oder eine Marke außerhalb von Collaboration zu bezeichnen. Der Begriff **Mitarbeiter** bezieht sich auf jedes Konto, das in Collaboration eine Verbindung herstellen kann, unabhängig davon, ob es sich um einen Advertiser oder einen Publisher handelt.

Im Marken-zu-Marken-Muster können sich zwei Marken, die außerhalb des Produkts kommuniziert haben, direkt in Collaboration über eine (private [) ](#private-connection-invite) verbinden. Eine Marke kann entweder ein Advertiser oder ein Publisher sein. Dieses Muster ist besonders für Marken nützlich, die nicht zum herkömmlichen Advertiser-Publisher-Modell passen, z. B. zwei Advertiser oder zwei Publisher.

Zunächst sendet ein Mitarbeiter eine private Verbindungseinladung an einen anderen Mitarbeiter. Der Empfänger prüft die Einladung und akzeptiert sie, sodass der Besitzer Verbindungseinstellungen vorschlagen kann. Sobald der Empfänger die Verbindungseinstellungen akzeptiert, wird die Verbindung hergestellt und beide Mitarbeiter können mit der Arbeit an Projekten beginnen.

### Allgemeine Übersicht

>[!TIP]
>
>Bei der Erörterung des Verbindungsprozesses wird zwischen dem **Eigentümer** und dem **Empfänger** unterschieden. Der Eigentümer ist der Mitarbeiter, der die Verbindung initiiert, indem er die Einladung sendet, während der Empfänger der Mitarbeiter ist, der die Einladung empfängt und überprüft.

Der Verbindungsprozess zwischen zwei Marken umfasst mehrere Schritte. Bevor der Verbindungsprozess beginnt, müssen einige Voraussetzungen erfüllt sein:

1. Zwei Marken kommunizieren außerhalb des Produkts, um die potenzielle Verbindung zu besprechen.
1. Die Marken [erstellen ](/help/guide/setup/onboard-account.md) in Collaboration, falls noch nicht geschehen, und achten darauf, den entsprechenden Rollentyp (Advertiser oder Publisher) auszuwählen.

   Sobald die Voraussetzungen erfüllt sind, kann der Verbindungsprozess gestartet werden. Die folgenden Schritte beschreiben den Prozess:

1. [Einladung zur privaten Verbindung senden](#send-private-connection-invite): Ein Mitarbeiter sendet eine Einladung zur privaten Verbindung an einen anderen Mitarbeiter.
1. [Einladung zur privaten Verbindung akzeptieren](#accept-private-connection-invite): Der Empfänger prüft und akzeptiert die Einladung zur privaten Verbindung.
1. [Verbindungseinstellungen konfigurieren](#configure-connection-settings): Der Eigentümer konfiguriert die Verbindungseinstellungen und sendet sie zur Überprüfung und Annahme an den Empfänger.
1. [Verbindungseinstellungen bestätigen](#establish-connection): Der Empfänger prüft die Verbindungseinstellungen und akzeptiert oder lehnt sie ab.

Sobald die Verbindungseinstellungen akzeptiert wurden, wird die Verbindung hergestellt und die Mitarbeiter können [ Projekt erstellen](/help/guide/collaborate/manage-projects.md#create-project) um mit der Zusammenarbeit bei Kampagnen zu beginnen.

## Verbinden {#connect}

Im **[!UICONTROL Connect]**-Arbeitsbereich können Sie Ihre Verbindungen mit Mitarbeitern verwalten, Verbindungseinladungen senden und Werbetreibende das Herausgeberverzeichnis durchsuchen. Der Arbeitsbereich ist in zwei Hauptregisterkarten unterteilt:

### Publisher entdecken {#discover-publishers}

>[!IMPORTANT]
>
>Nur Werbetreibende können Publisher mithilfe des Arbeitsbereichs **[!UICONTROL Discover Publishers]** finden. Informationen zur Verbindung mit Partnern unabhängig von ihrer Rolle finden Sie [ Abschnitt „Marke-zu-Marke-Verbindung](#brand-to-brand-connection).

Um Herausgeber zu finden, navigieren Sie auf der Registerkarte **[!UICONTROL Verbinden]** zum Arbeitsbereich **[!UICONTROL Herausgeber]**. Hier können Sie die Liste der verfügbaren Herausgeber mithilfe der Steuerelemente für die Paginierung unten im Arbeitsbereich durchsuchen. Weitere Informationen zum Arbeitsbereich **[!UICONTROL Discover Publishers]** finden Sie im Handbuch [Discover Publishers](/help/guide/connect/discover-publishers.md) .

![Der Arbeitsbereich „Publisher suchen“ mit einer Liste der verfügbaren Publisher.](/help/assets/connect/establish-connection/discover-publishers.png){zoomable="yes"}

### Einladung senden {#send-invite}

>[!IMPORTANT]
>
>In diesem Abschnitt wird der Prozess beschrieben, bei dem Advertiser über den Arbeitsbereich **[!UICONTROL Discover Publishers“ Verbindungseinladungen an]** senden. Um mehr über die Bildung von Verbindungen zwischen Marken zu erfahren, unabhängig von deren Rollen, lesen Sie den Abschnitt [Marke-zu-Marke-Verbindung](#brand-to-brand-connection) oder besuchen Sie den Abschnitt [Einladung zur privaten Verbindung](#private-connection-invite).

Nachdem Sie einen Herausgeber identifiziert haben, mit dem Sie zusammenarbeiten möchten, wählen Sie die **[!UICONTROL Verbinden]** auf der Herausgeberkarte. Diese Aktion initiiert den Verbindungsprozess.

![Die hervorgehobene Option „Verbinden“ für einen bestimmten Herausgeber im Arbeitsbereich „Herausgeber suchen“.](/help/assets/connect/establish-connection/connect-selection.png){zoomable="yes"}

Es wird ein Dialogfeld angezeigt, in dem Sie aufgefordert werden, eine Einladung zur Verbindung an den Herausgeber zu senden. Wählen Sie **[!UICONTROL Einladung senden]** um fortzufahren.

![Das Dialogfeld „Einladung für Verbindung senden“ mit hervorgehobener Schaltfläche „Einladung senden“.](/help/assets/connect/establish-connection/send-connection-invite-dialog.png){zoomable="yes"}

>[!NOTE]
>
>Wenn Sie eine Verbindung zu einem Herausgeber herstellen möchten, mit dem Sie außerhalb des Produkts kommuniziert haben, können Sie die Option Einladung zur privaten Verbindung verwenden. Weitere Informationen finden Sie im Abschnitt [Einladung zur privaten Verbindung](#private-connection-invite).

Die ausstehende Einladung wird auf der Registerkarte **[!UICONTROL Meine Verbindungen]** im Abschnitt **[!UICONTROL Aktion erforderlich]** angezeigt. Der Verbindungsstatus wird als &quot;**[!UICONTROL gesendet“]**. Sie können die Verbindungseinstellungen in der Vorschau anzeigen, indem Sie **[!UICONTROL Verbindung in der Vorschau anzeigen]** auswählen. Sie können sie jedoch erst bearbeiten, wenn der Publisher die Einladung akzeptiert.

![Die ausstehende Verbindung wird im Arbeitsbereich Meine Verbindungen im Abschnitt Erforderliche Aktion angezeigt.](/help/assets/connect/establish-connection/preview-connection.png){zoomable="yes"}

### Private Verbindungseinladung {#private-connection-invite}

Private Verbindungseinladungen ermöglichen es Ihnen, sich mit Mitarbeitern, mit denen Sie außerhalb des Produkts kommuniziert haben, über einen &quot;**[!UICONTROL -Code“]** verbinden. Um eine private Verbindung zu erstellen, müssen Sie den **[!UICONTROL Connect-Code]** von dem Mitarbeiter abrufen, mit dem Sie außerhalb des Produkts eine Verbindung herstellen möchten. Sie können diesen Code dann verwenden, um eine Einladung zur privaten Verbindung an den Mitarbeiter im Arbeitsbereich **[!UICONTROL Verbinden]** zu senden.

#### Verbindungs-Code {#connect-code}

Bevor Sie eine private Verbindungseinladung senden können, muss Ihr gewünschter Mitarbeiter Ihnen seinen eindeutigen **[!UICONTROL Connect-Code]** bereitstellen. Navigieren Sie zum Suchen und Kopieren Ihres **[!UICONTROL Verbindungs]**&#x200B;**[!UICONTROL Codes im]**-Arbeitsbereich zur **[!UICONTROL Mein Konto]** . Der **[!UICONTROL Connect-Code]** wird in Ihren Kontodetails angezeigt.

![Die Registerkarte „Mein Konto“ im Arbeitsbereich „Setup“ mit hervorgehobenem Verbindungs-Code.](/help/assets/connect/establish-connection/connect-code.png){zoomable="yes"}

Wählen Sie das Kopiersymbol (![Kopiersymbol](/help/assets/icons/copy.png)) neben dem **[!UICONTROL Code verbinden]**, um ihn in die Zwischenablage zu kopieren. Sie können diesen Code dann außerhalb des Produkts für Ihren Mitwirkenden freigeben.

![Der Code „Verbinden“ mit hervorgehobenem Kopiersymbol.](/help/assets/connect/establish-connection/copy-connect-code.png){zoomable="yes"}

##### Verbindungscode wird aktualisiert {#refresh-connect-code}

Sie können Ihren **[!UICONTROL Connect-Code]** jederzeit aktualisieren. Durch Aktualisieren des Codes wird ein neuer eindeutiger Code generiert, den Sie für Mitwirkende freigeben können. Dies ist nützlich, wenn Sie den vorherigen Code aus Sicherheitsgründen ungültig machen möchten. Alle Verbindungen, die mit dem alten Code hergestellt wurden, bleiben aktiv, aber neue Mitarbeiter müssen den neuen Code verwenden, um eine Verbindung mit Ihnen herzustellen.

>[!IMPORTANT]
>
>Wenn Sie Ihren **[!UICONTROL Connect-Code]** während einer ausstehenden Einladung aktualisieren, kann dies verhindern, dass die Einladung angenommen wird. Wenn Sie Ihren Code aktualisieren, muss Ihr Mitarbeiter möglicherweise die private Verbindungseinladung erneut mit dem neuen Code senden.

Um Ihren **[!UICONTROL Verbindungs-Code]** zu aktualisieren, klicken Sie auf das Aktualisierungssymbol (![Aktualisierungssymbol](/help/assets/icons/refresh.png)) neben dem **[!UICONTROL Verbindungs-Code]**.

![Der Code „Verbinden“ mit hervorgehobenem Aktualisierungssymbol.](/help/assets/connect/establish-connection/refresh-connect-code.png){zoomable="yes"}

>[!IMPORTANT]
>
>Konten, die vor der Einführung der Funktion **[!UICONTROL Code verbinden]** erstellt wurden, haben keinen generierten Verbindungscode und das Feld „Verbinden“ wird als &quot;**[!UICONTROL verfügbar“]**. Verwenden Sie die Aktualisierungsoption, um einen neuen Verbindungs-Code zu generieren.

#### Einladung zur privaten Verbindung senden {#send-private-connection-invite}

Sobald Sie den **[!UICONTROL Connect-Code]** von Ihrem Mitarbeiter haben, können Sie eine Einladung für eine private Verbindung senden. Navigieren Sie dazu zum Arbeitsbereich **[!UICONTROL Verbinden]** und wählen Sie das Pluszeichen (![Pluszeichen](/help/assets/icons/plus.png)) oben rechts aus.

![Das Pluszeichen, das im Arbeitsbereich „Verbinden“ hervorgehoben ist.](/help/assets/connect/establish-connection/private-connection-invite.png){zoomable="yes"}

Das **[!UICONTROL Verbinden]**-Dialogfeld erscheint, in dem Sie aufgefordert werden, den **[!UICONTROL Verbinden-Code]** des Mitarbeiters einzugeben, mit dem Sie eine Verbindung herstellen möchten. Fügen Sie den Code in das Textfeld ein und wählen Sie **[!UICONTROL Weiter]**, um fortzufahren.

![Das Dialogfeld „Verbinden“ mit ausgefülltem Feld „Code verbinden“ und hervorgehobener Option „Weiter“.](/help/assets/connect/establish-connection/private-connection-invite-connect.png){zoomable="yes"}

Im **[!UICONTROL Verbinden]**-Dialogfeld wird dann der Mitarbeiter angezeigt, mit dem der Code verknüpft ist, sodass Sie bestätigen können, dass Sie eine Verbindung mit dem richtigen Mitarbeiter herstellen. Wenn der Mitarbeiter korrekt ist, wählen Sie **[!UICONTROL Verbinden]** aus, um die Einladung zur privaten Verbindung zu senden.

![Das Dialogfeld „Verbinden“ mit den angezeigten Mitarbeiterdetails und der hervorgehobenen Option „Verbinden“.](/help/assets/connect/establish-connection/private-connection-invite-connect-confirm.png){zoomable="yes"}

### Einladung annehmen {#accept-invite}

>[!TIP]
>
>Bei der Erörterung des Verbindungsprozesses wird zwischen dem **Eigentümer** und dem **Empfänger** unterschieden. Der Eigentümer ist der Mitarbeiter, der die Verbindung initiiert, indem er die Einladung sendet, während der Empfänger der Mitarbeiter ist, der die Einladung empfängt und überprüft.

Bevor der Eigentümer die Verbindungseinstellungen konfigurieren kann, muss der Empfänger die Verbindungseinladung annehmen. Navigieren Sie dazu zum Arbeitsbereich **[!UICONTROL Verbinden]** und suchen Sie im Abschnitt **[!UICONTROL Aktion erforderlich]** nach der ausstehenden Verbindung. Der Verbindungsstatus wird als &quot;**[!UICONTROL empfangen“]**. Wählen **[!UICONTROL Akzeptieren]** aus, um die Einladung anzunehmen.

![Die ausstehende Verbindung wird im Abschnitt Aktion erforderlich des Arbeitsbereichs „Verbinden“ angezeigt, wobei die Option Akzeptieren hervorgehoben ist.](/help/assets/connect/establish-connection/accept-connection.png){zoomable="yes"}

Das Dialogfeld erscheint, in dem Sie aufgefordert werden, die Einladung anzunehmen. Wählen Sie **[!UICONTROL Einladung annehmen]** um fortzufahren.

![Das Dialogfeld „Einladung zur Verbindung annehmen“ mit hervorgehobener Option „Einladung annehmen“.](/help/assets/connect/establish-connection/accept-connection-invite.png){zoomable="yes"}

Der Status der Verbindung ändert sich in **[!UICONTROL Ausstehend]**. Der Inhaber kann jetzt die Verbindungseinstellungen konfigurieren.

### Konfigurieren der Verbindungseinstellungen {#configure-connection-settings}

Die Verbindungseinstellungen definieren die Begriffe zwischen zwei Mitwirkenden. Zu diesen Einstellungen gehören Anwendungsfälle, Übereinstimmungsschlüssel, Kreditaufteilung und rechtliche Vereinbarungen. Mitarbeiter, die eine Verbindung zu Werbetreibenden herstellen, können auch Werbekunden-Namen zu den Verbindungseinstellungen hinzufügen, die beim Erstellen von Projekten verwendet werden.

Nachdem der Empfänger die Einladung akzeptiert hat, kann der Besitzer die Verbindungseinstellungen konfigurieren. Navigieren Sie dazu zu &quot;**[!UICONTROL Verbindungen“]** suchen Sie die ausstehende Verbindung im Abschnitt **[!UICONTROL Aktion erforderlich]** . Wählen Sie **[!UICONTROL Verbindung einrichten]** aus, um die Verbindungseinstellungen zu konfigurieren.

![Der Arbeitsbereich „Verbinden“ mit der hervorgehobenen Option „Verbindung einrichten“ im Abschnitt Erforderliche Aktion.](/help/assets/connect/establish-connection/pending-connection.png){zoomable="yes"}

Der Arbeitsbereich Verbindungseinstellungen wird angezeigt, in dem Sie die verschiedenen Einstellungen für die Verbindung konfigurieren können.

![Der Arbeitsbereich „Verbindungseinstellungen“](/help/assets/connect/establish-connection/connection-set-up.png){zoomable="yes"}

#### Verbindungseinstellungen {#connection-settings}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_usecases"
>title="Anwendungsfälle"
>abstract="Die Anwendungsszenarien sind mit allen Optionen vorausgefüllt. Die Anwendungsszenarien können bearbeitt werden, bevor die Verbindungseinstellungen übermittelt werden."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_matchkeys"
>title="Übereinstimmungsschlüssel"
>abstract="Übereinstimmungsschlüssel werden mit allgemeinen Übereinstimmungsschlüsseln vorausgefüllt, die Sie und die mitwirkende Person auf Kontoebene ausgewählt haben. Alle Übereinstimmungsschlüssel, die in dieser Verbindung nicht verwendet werden sollen, können deaktiviert werden."
>additional-url="https://experienceleague.adobe.com/de/docs/real-time-cdp-collaboration/using/setup/onboard-account#set-up-match-keys" text="Übereinstimmungsschlüssel für Konten"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit"
>title="Kostenaufteilung"
>abstract="In diesem Abschnitt wird festgelegt, wer die Kosten für die entsprechenden Aktivitäten in Collaboration trägt. "

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="Freigabe von Zielgruppen"
>abstract="Credits für die Zielgruppenaktivierung werden basierend auf der Anzahl der übereinstimmenden IDs verwendet, die für die Aktivierung vorbereitet wurden."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_measurement"
>title="Messung"
>abstract="Ausführen von Aktivitäten zum Generieren von Leistungsberichten und Erkenntnissen für Kampagnen. Die Credits werden basierend auf der Anzahl der Zeilen in allen Kampagnenberichten und der Reporting-Häufigkeit (täglich, alle drei Tage oder wöchentlich) verwendet."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_advertisername"
>title="Advertiser-Namen"
>abstract="<p>Optionale Einstellung. Gibt den Namen und die ID an, unter denen der Advertiser dem Publisher bekannt ist.</p><p>Der hier hinzugefügte Advertiser-Name wird im Schritt „Projekt erstellen“ vorausgefüllt.</p><ul><li>Wenn der Publisher mehrere Namen konfiguriert hat, wählen Sie einen aus der Liste aus.</li><li>Wenn nur ein Name konfiguriert ist, wird er automatisch vorausgewählt.</li><li>Wenn keine Namen konfiguriert sind, wird das Feld mit dem Advertiser-Kontonamen aus Collaboration vorausgefüllt.</li></ul>"
>additional-url="https://experienceleague.adobe.com/de/docs/real-time-cdp-collaboration/using/collaborate/manage-projects#create-project" text="Erstellen eines Projekts"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_audience_activation"
>title="Zielgruppenaktivierung"
>abstract="Mit der Zielgruppenaktivierung können Sie auswählen, welche mitwirkende Person die Zielgruppenaktivierung initiieren kann."

Sie können die folgenden Verbindungseinstellungen konfigurieren:

##### Zielgruppenaktivierung {#audience-activation}

>[!IMPORTANT]
>
>Für alle Verbindungen, die vor der Einführung **[!UICONTROL Funktion]** Zielgruppenaktivierung“ erstellt wurden, ist die Einstellung für die Zielgruppenaktivierung automatisch auf den Verbindungsbesitzer festgelegt. Wenn Sie beiden Mitarbeitern erlauben möchten, Zielgruppen zu aktivieren, müssen Sie [Ihre aktuelle Verbindung löschen](#delete-connections) und eine neue mit den aktualisierten Einstellungen erstellen.

Mit der Zielgruppenaktivierung können Sie auswählen, welcher Mitarbeiter Zielgruppen in der Verbindung aktivieren kann. Die Zielgruppenaktivierung ist nur eine Option, wenn der Anwendungsfall **[!UICONTROL Zielgruppenaktivierung]** ausgewählt ist. Wenn Sie sich dafür entscheiden, den Anwendungsfall während des Verbindungsprozesses zu entfernen, wird die Zielgruppen-Aktivierungseinstellung aus den Verbindungseinstellungen entfernt. Weitere Informationen zur Aktivierung von Zielgruppen finden Sie im [aktivieren](/help/guide/collaborate/activate.md)-Handbuch.

Um die Zielgruppenaktivierung einzurichten, wählen Sie **[!UICONTROL Einrichten]** im Abschnitt **[!UICONTROL Zielgruppenaktivierung]** aus. Verwenden Sie das Dropdown-Menü, um festzulegen, welcher Mitarbeiter Zielgruppen aktivieren kann. Sie können einen einzelnen Mitarbeiter auswählen oder beiden Mitarbeitern erlauben, Zielgruppen zu aktivieren.

![Das Dialogfeld für die Zielgruppenaktivierung mit Optionen im Arbeitsbereich „Verbindungseinstellungen“](/help/assets/connect/establish-connection/audience-activation.png){zoomable="yes"}

Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Speichern]**, um Ihre Änderungen zu speichern.

![Das Dialogfeld für die Zielgruppenaktivierung mit der Option Speichern im Arbeitsbereich „Verbindungseinstellungen“.](/help/assets/connect/establish-connection/audience-activation-confirm.png){zoomable="yes"}

##### Anwendungsfälle {#use-cases}

Anwendungsfälle werden automatisch mit allen verfügbaren Optionen ausgefüllt. Ausgewählte Anwendungsfälle bestimmen, welche Ansichten und Optionen in Ihren Projekten verfügbar sind. Weitere Informationen finden Sie im [Projekt-Anwendungsfälle](/help/guide/collaborate/manage-projects.md#project-use-cases)Handbuch.

Um Ihre Anwendungsfälle anzupassen, wählen Sie **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Anwendungsfälle]** und deaktivieren Sie alle, die Sie nicht in Projekte mit Ihrem Mitarbeiter aufnehmen möchten. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Speichern]**, um Ihre Änderungen zu speichern.

![Die Einstellungen für Anwendungsfälle im Arbeitsbereich „Verbindungseinstellungen“.](/help/assets/connect/establish-connection/view-use-cases.png){zoomable="yes"}

##### Übereinstimmungsschlüssel {#match-keys}

>[!IMPORTANT]
>
>Beim Aktivieren von Zielgruppen, für die mehrere Übereinstimmungsschlüssel verwendet werden, schlägt die gesamte Aktivierung fehl, wenn ein (oder mehrere) Übereinstimmungsschlüssel keine Überschneidungen aufweisen, keine Zielgruppen zählen oder unter den Schwellenwert fallen. Stellen Sie vor der Aktivierung sicher, dass sich Ihre Zielgruppen ausreichend überschneiden und der Mindestschwellenwert von 1.000 IDs für alle Übereinstimmungsschlüssel erreicht wird.

Übereinstimmungsschlüssel werden automatisch mit den allgemeinen Übereinstimmungsschlüsseln ausgefüllt, die Sie und Ihr Mitarbeiter beim [Einrichten Ihrer Konten“ ausgewählt ](/help/guide/setup/onboard-account.md#set-up-match-keys). Es werden nur Übereinstimmungsschlüssel angezeigt, die sowohl von Ihnen als auch **ausgewählten** gemeinsam haben.

![Der Arbeitsbereich „Verbindungseinstellungen“ mit hervorgehobenem Abschnitt „Übereinstimmungsschlüssel“, in dem die allgemeinen Übereinstimmungsschlüssel angezeigt werden.](/help/assets/connect/establish-connection/auto-populated-match-keys.png){zoomable="yes"}

Wenn der Verbindungsbesitzer die Verbindungseinstellungen einrichtet, kann er [seine Konto-Übereinstimmungsschlüssel bearbeiten](../setup/onboard-account.md#edit-match-keys) um zusätzliche Übereinstimmungsschlüssel einzuschließen. Nachdem Sie weitere Übereinstimmungsschlüssel in Ihren Kontoeinstellungen aktiviert haben, können diese Übereinstimmungsschlüssel in den Verbindungseinstellungen aktiviert werden, wenn Ihr Mitarbeiter sie ebenfalls ausgewählt hat. Übereinstimmungsschlüssel, die hinzugefügt wurden, sobald der Verbindungsprozess begonnen hat, werden nicht automatisch ausgefüllt und müssen manuell aktiviert werden.

Um Ihre Übereinstimmungsschlüssel anzupassen, wählen **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Übereinstimmungsschlüssel]** und schalten Sie alle Übereinstimmungsschlüssel aus, die Sie in dieser Verbindung nicht verwenden möchten. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Speichern]**, um Ihre Änderungen zu speichern.

![Der Arbeitsbereich „Verbindungseinstellungen“ mit dem Abschnitt „Übereinstimmungsschlüssel“ wird geöffnet und zeigt einen umgeschalteten Übereinstimmungsschlüssel an.](/help/assets/connect/establish-connection/additional-match-key-selected.png){zoomable="yes"}

>[!IMPORTANT]
>
>Sobald Ihr Mitarbeiter die Verbindungseinstellungen akzeptiert hat, werden die Übereinstimmungsschlüssel gesperrt und können nicht mehr geändert werden.

##### Kostenaufteilung {#credit-split}

Verwenden Sie den Abschnitt „Kreditaufteilung“, um zu bestimmen, welche der beiden kooperierenden Parteien die Kosten für die Aktivitäten deckt. Die Optionen für die Kreditaufteilung werden durch die ausgewählten Anwendungsfälle für die Verbindung bestimmt. Während im **[!UICONTROL Measurement]**-Anwendungsfall eine Partei die Kosten decken muss, bietet der **[!UICONTROL Activation - Matching]**-Anwendungsfall eine zusätzliche Option, damit jede Partei ihre eigenen Kosten übernimmt. Informationen zur Kostenaufschlüsselung finden Sie im Handbuch [Arten von ](/help/guide/setup/my-activity.md#types-of-activities)).

>[!NOTE]
>
>Zielgruppe - Der Ausgang wird immer von dem Mitarbeiter abgedeckt, der die Zielgruppe erhält. Daher ist keine Auswahl erforderlich.

Um die Kreditaufteilung einzurichten, wählen Sie **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Kreditaufteilung]** aus. Anschließend können Sie für jeden Anwendungsfall die entsprechenden Optionen auswählen. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Speichern]**, um Ihre Änderungen zu speichern.

![Das Dialogfeld „Kreditaufteilung“ mit Optionen im Arbeitsbereich „Verbindungseinstellungen“.](/help/assets/connect/establish-connection/credit-split.png){zoomable="yes"}

##### Advertiser-Namen {#advertiser-names}

>[!NOTE]
>
>Je nachdem, wer die Verbindung initiiert, kann diese Option während der Konfiguration der Verbindungseinstellungen oder der Überprüfung der Verbindungseinstellungen angezeigt werden.

Wenn Sie ein Publisher sind und eine Verbindung mit einem Advertiser herstellen, können Sie in den Verbindungseinstellungen Advertiser-Namen hinzufügen. Auf diese Weise können Sie mehrere Namen hinzufügen, mit denen der Advertiser Ihnen in Ihren Systemen bekannt ist. Dies ist besonders nützlich, wenn der Werbetreibende in mehreren Regionen präsent ist oder wenn er unter verschiedenen Namen in verschiedenen Kontexten bekannt ist. Wenn Sie später ein Projekt erstellen, können Sie den entsprechenden Advertiser-Namen aus der Liste der in den Verbindungseinstellungen konfigurierten Namen auswählen.

![Die Advertiser-Namen im Arbeitsbereich „Verbindungseinstellungen“](/help/assets/connect/establish-connection/advertiser-names.png){zoomable="yes"}

Um Advertiser-Namen hinzuzufügen, wählen **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Advertiser-Namen]** aus. Sie können dann die **[!UICONTROL Advertiser-ID]**, die Ihnen der Advertiser in Ihrem System genannt wird, und einen **[!UICONTROL Advertiser-Namen]** eingeben, der mit dieser ID in Collaboration verknüpft werden soll. Sie können mehrere Advertiser-Namen hinzufügen, indem Sie die Option **[!UICONTROL Hinzufügen]** auswählen.

![Das Dialogfeld „Advertiser-Namen“ mit Optionen im Arbeitsbereich „Verbindungseinstellungen“.](/help/assets/connect/establish-connection/advertiser-names-dialog.png){zoomable="yes"}

Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Speichern]**, um Ihre Änderungen zu speichern.

Beim Erstellen eines Projekts wird der Advertiser-Name basierend auf den folgenden Einstellungen, die während der Verbindung festgelegt wurden, vorbefüllt    :

1. **Kein Advertiser-Name festgelegt**: Wenn keine Advertiser-Namen hinzugefügt werden, verwendet Collaboration standardmäßig den Namen des Advertisers als Advertiser-Namen.
2. **Ein Werbekunden-Name festgelegt**: Wenn ein einzelner Werbekunden-Name hinzugefügt wird, verwendet Collaboration diesen Namen automatisch als Werbekunden-Name für das Projekt.
3. **Mehrere Advertiser-Namen festgelegt**: Wenn mehr als ein Advertiser-Name hinzugefügt wird, können Sie oder Ihr Mitarbeiter beim Erstellen des Projekts einen der angegebenen Namen auswählen.

>[!NOTE]
>
> Nachdem Sie die Verbindungseinstellungen gesendet haben, können Sie keine Advertiser-Namen mehr hinzufügen oder bearbeiten.

![Der Arbeitsbereich „Verbindungseinstellungen“ mit ausgefülltem Abschnitt „Advertiser-Namen“.](/help/assets/connect/establish-connection/add-advertiser-names.png)

Nachdem Sie Ihre Auswahl getroffen haben, wählen Sie **[!UICONTROL Senden]** aus, um die vorgeschlagenen Einstellungen zur Überprüfung an den Empfänger zu senden.

### Verbindungseinstellungen überprüfen {#review-connection-settings}

Als Nächstes muss der Empfänger die vom Eigentümer vorgeschlagenen Verbindungseinstellungen überprüfen. Der Empfänger kann dies tun, indem er zur Registerkarte **[!UICONTROL Meine Verbindungen]** im Arbeitsbereich **[!UICONTROL Verbinden]** navigiert. Die Verbindung wird im Abschnitt **[!UICONTROL Aktion erforderlich]** angezeigt. Wählen Sie **[!UICONTROL Verbindungseinstellungen überprüfen]** aus, um die vorgeschlagenen Verbindungseinstellungen zu überprüfen.

![Der Arbeitsbereich „Meine Verbindungen“ mit hervorgehobener Option „Verbindungseinstellungen überprüfen“.](/help/assets/connect/establish-connection/review-connection-settings.png){zoomable="yes"}

Überprüfen Sie die Einstellungen, die der Mitarbeiter vorgeschlagen hat. Sie können die Verbindungseinstellungen entweder akzeptieren oder ablehnen. Wenn Sie die Verbindungseinstellungen ablehnen, müssen Sie mit dem Mitarbeiter über die Änderungen kommunizieren, die Sie außerhalb des Produkts vornehmen möchten. Die Kontaktinformationen des Mitarbeiters werden im Abschnitt **[!UICONTROL Kontakt]** des Arbeitsbereichs Verbindungseinstellungen angezeigt. Der Besitzer kann dann die Verbindungseinstellungen überarbeiten und zur Überprüfung erneut senden.

![Der Arbeitsbereich „Verbindungseinstellungen“ mit hervorgehobener Option „Akzeptieren“ und „Ablehnen“.](/help/assets/connect/establish-connection/accept-connection-settings.png){zoomable="yes"}

Wenn Sie ein Herausgeber sind, der eine Verbindung zu einem Advertiser herstellt, können Sie jetzt Advertiser-Namen in den Verbindungseinstellungen hinzufügen. Weitere Informationen zu diesem Prozess finden Sie [ Abschnitt &quot;](#connection-settings)&quot;.

>[!NOTE]
>
> Nachdem Sie die Verbindungseinstellungen akzeptiert haben, können Sie keine Advertiser-Namen mehr hinzufügen oder bearbeiten.

Wählen Sie als Nächstes **[!UICONTROL Akzeptieren]** aus, um mit der Verbindung fortzufahren. Der Verbindungsstatus ändert sich in **[!UICONTROL Aktiv]** und Sie können jetzt mit der Zusammenarbeit an Projekten beginnen.

## Verbindungen löschen {#delete-connections}

Sie können alle Verbindungen mit Partnern löschen, mit denen Sie nicht weiter arbeiten möchten. Um vorhandene Verbindungen zu löschen, navigieren Sie zu **[!UICONTROL Verbinden]**. Als Herausgeber wird Ihre bestehende Verbindung angezeigt. Als Werbetreibender sollten Sie dann zu &quot;**[!UICONTROL Verbindungen“]**.

Wählen **[!UICONTROL auf]** Verbindungskarte, die Sie löschen möchten, die Option „Verbindung anzeigen“ aus.

![Die Option „Verbindung anzeigen“, die in der Ansicht „Meine Verbindungen“ hervorgehoben ist.](/help/assets/connect/establish-connection/delete-view-connection.png){zoomable="yes"}

Wählen Sie das Löschsymbol ![Löschsymbol](/help/assets/common/delete.svg) im Arbeitsbereich „Verbindung“ aus, um die Verbindung zu löschen.

![Das hervorgehobene Löschsymbol im Arbeitsbereich „Verbindung“.](/help/assets/connect/establish-connection/delete-option.png){zoomable="yes"}

Es wird ein Bestätigungsdialogfeld angezeigt, in dem Sie aufgefordert werden, das Löschen der Verbindung zu bestätigen. Wählen Sie **[!UICONTROL Löschen]** aus, um den Löschvorgang zu bestätigen.

![Das Bestätigungsdialogfeld zum Löschen einer Verbindung.](/help/assets/connect/establish-connection/delete-confirmation-dialog.png){zoomable="yes"}

>[!WARNING]
>
>Sobald die Verbindung gelöscht ist, werden alle vorhandenen Projekte in der Zusammenarbeit dauerhaft gelöscht und können nicht wiederhergestellt werden. Die Verbindungsanfrage verbleibt in einem ausstehenden Status, aber die Verbindung und ihre Konfigurationen sind nicht mehr aktiv. Sie müssen die Verbindung wiederherstellen, wenn Sie erneut eine Verbindung mit dem Mitarbeiter herstellen möchten.

## Nächste Schritte

Nachdem Sie eine Verbindung mit Ihrem Mitarbeiter hergestellt haben, können Sie und Ihr Mitarbeiter jetzt [Projekte erstellen](/help/guide/collaborate/manage-projects.md#create-project).
