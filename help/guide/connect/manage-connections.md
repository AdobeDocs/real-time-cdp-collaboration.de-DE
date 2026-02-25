---
title: Verwalten von Verbindungen
description: Erfahren Sie, wie Sie Ihre Verbindungen in Real-Time CDP Collaboration verwalten.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 50120839-4a20-4ec1-8887-9342bd17c52d
source-git-commit: 46d2596bd0ccdc5da32067493968945c61f8acc4
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 1%

---

# Verwalten von Verbindungen {#manage-connections}

{{limited-availability-release-note}}

Der **[!UICONTROL Meine Verbindungen]** Arbeitsbereich bietet einen zentralen Speicherort für die Verwaltung Ihrer Verbindungen. Sie können vorhandene Verbindungen im Abschnitt **[!UICONTROL Vorhandene Verbindungen]** anzeigen und alle Verbindungen, die eine Aktion erfordern, im Abschnitt **[!UICONTROL Aktion erforderlich]** anzeigen.

## Verbindung anzeigen {#view-connection}

Um Ihre vorhandenen Verbindungen anzuzeigen, navigieren Sie zum Arbeitsbereich **[!UICONTROL Verbinden]** . Als Herausgeber wird Ihre bestehende Verbindung angezeigt. Als Werbetreibender sollten Sie dann zu &quot;**[!UICONTROL Verbindungen“]**.

![Die hervorgehobene Option „Verbindung anzeigen“ für eine Verbindung im Arbeitsbereich „Meine Verbindungen“.](/help/assets/connect/manage-connections/view-connection.png){zoomable="yes"}

Der Arbeitsbereich „Verbindungsübersicht“ wird mit Details zur Verbindung und zu ihren aktiven Projekten angezeigt. Wählen Sie **[!UICONTROL Verbindungseinstellungen]** aus, um die Verbindungseinstellungen anzuzeigen.

![Die hervorgehobene Option „Verbindungseinstellungen“ im Arbeitsbereich „Verbindungsübersicht“.](/help/assets/connect/manage-connections/connection-overview.png){zoomable="yes"}

Der Arbeitsbereich Verbindungseinstellungen wird angezeigt, in dem die Verbindungsdetails zwischen Ihnen und Ihrem Mitarbeiter angezeigt werden. Hier können Sie alle während des Verbindungsprozesses ausgewählten Einstellungen, den aktuellen Status der Verbindung, den Verbindungseigentümer und die Kontaktinformationen für Ihren Mitarbeiter anzeigen. Informationen zu bestimmten Verbindungseinstellungen finden Sie im [Verbindungseinstellungen](/help/guide/connect/establishing-connections.md#connection-settings).

![Der Arbeitsbereich „Verbindungseinstellungen“ mit Verbindungsdetails.](/help/assets/connect/manage-connections/connection-settings.png){zoomable="yes"}

## Verbindung löschen {#delete-connection}

Sie können alle Verbindungen mit Partnern löschen, mit denen Sie nicht weiter arbeiten möchten. Um eine Verbindung zu löschen, navigieren Sie zu der Verbindung, die Sie löschen möchten, und wählen Sie dann im Arbeitsbereich Verbindung das Symbol „Löschen![ (](/help/assets/common/delete.svg)) aus.

![Das hervorgehobene Löschsymbol im Arbeitsbereich „Verbindung“.](/help/assets/connect/establish-connection/delete-option.png){zoomable="yes"}

Es wird ein Bestätigungsdialogfeld angezeigt, in dem Sie aufgefordert werden, das Löschen der Verbindung zu bestätigen. Wählen Sie **[!UICONTROL Löschen]** aus, um den Löschvorgang zu bestätigen.

![Das Bestätigungsdialogfeld zum Löschen einer Verbindung.](/help/assets/connect/establish-connection/delete-confirmation-dialog.png){zoomable="yes"}

>[!WARNING]
>
>Sobald die Verbindung gelöscht ist, werden alle vorhandenen Projekte in der Zusammenarbeit dauerhaft gelöscht und können nicht wiederhergestellt werden. Die Verbindungsanfrage verbleibt im Abschnitt **[!UICONTROL Aktion erforderlich]** unter **[!UICONTROL Meine Verbindungen]** im ausstehenden Status, aber die Verbindung und ihre Konfigurationen sind nicht mehr aktiv. Sie müssen die Verbindung wiederherstellen, wenn Sie erneut eine Verbindung mit dem Mitarbeiter herstellen möchten.

## Verbindung bearbeiten {#edit-connection}

Als Verantwortlicher für eine Collaboration-Verbindung können Sie die Verbindungseinstellungen mit Ihrem Verantwortlichen bearbeiten, nachdem die Verbindung hergestellt wurde. Sie haben folgende Möglichkeiten:

* Anwendungsfälle hinzufügen
* Übereinstimmungsschlüssel hinzufügen. Das Entfernen von Übereinstimmungsschlüsseln wird in Zukunft unterstützt.
* Berechtigungen zur Zielgruppenaktivierung aktualisieren
* Kreditaufteilungseinstellungen aktualisieren

>[!IMPORTANT]
>
>Nachdem ein Anwendungsfall oder Übereinstimmungsschlüssel zu einer Verbindung hinzugefügt wurde, kann er nicht mehr entfernt werden.

>[!TIP]
>
>Der **Inhaber** ist der Mitarbeiter, der die Verbindung initiiert, indem er die Einladung an den (Empfänger **sendet**. Weitere Informationen finden Sie in der Dokumentation [Herstellen von Verbindungen mit Partnern](./establishing-connections.md).

Um Verbindungseinstellungen zu bearbeiten, navigieren Sie zum Arbeitsbereich Verbindungseinstellungen . Wählen Sie das Drei-Punkte![Symbol (Drei Punkte) aus.](/help/assets/icons/more.png)), um verfügbare Aktionen anzuzeigen, und wählen Sie dann **[!UICONTROL Bearbeiten]**.

![Der Arbeitsbereich „Verbindungseinstellungen“ mit hervorgehobener Option „Bearbeiten“.](/help/assets/connect/manage-connections/edit-connection.png){zoomable="yes"}

Ein Dialogfeld wird angezeigt, in dem Sie aufgefordert werden, die Einstellungsänderungen zu bearbeiten und zur Überprüfung durch den Mitarbeiter zu übermitteln. Wählen Sie **[!UICONTROL Bearbeiten]** aus.

![Das Dialogfeld „Verbindungseinstellungen bearbeiten“ mit hervorgehobener Option „Bearbeiten“.](/help/assets/connect/manage-connections/edit-connection-settings-dialog.png){zoomable="yes"}

### Audience-Aktivierung bearbeiten {#edit-audience-activation}

Die Einstellungen für die Zielgruppenaktivierung bestimmen, welcher Mitarbeiter in der Verbindung Zielgruppen für Ziele aktivieren kann. Um diese Einstellungen zu ändern, wählen Sie **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Zielgruppenaktivierung]** aus.

![Der Bildschirm „Verbindungseinstellungen bearbeiten“ mit dem Abschnitt Zielgruppenaktivierung und der Option „Bearbeiten“.](/help/assets/connect/manage-connections/edit-audience-activation.png){zoomable="yes"}

Aktualisieren Sie **[!UICONTROL Dialogfeld]** Zielgruppenaktivierung“ im Dropdown-Menü die Berechtigungen für die Zielgruppenaktivierung. Sie können einen einzelnen Mitarbeiter auswählen oder beiden Mitarbeitern erlauben, Zielgruppen zu aktivieren.

![Das hervorgehobene Dropdown-Menü „Zielgruppenaktivierung“ wurde erweitert, um die Berechtigungen zur Zielgruppenaktivierung zu aktualisieren.](/help/assets/connect/manage-connections/audience-activation-dropdown-menu.png){zoomable="yes"}

Klicken Sie abschließend auf **[!UICONTROL Speichern]**.

![Das Dialogfeld für die Zielgruppenaktivierung mit den neuen Zielgruppenaktivierungsberechtigungen und der Option „Speichern“.](/help/assets/connect/manage-connections/audience-activation-dialog.png){zoomable="yes"}

### Anwendungsfälle hinzufügen {#add-use-cases}

In Collaboration bestimmen Anwendungsfälle wie „Entdecken“, „Aktivieren“ und „Messen“, welche Projektabschnitte und Funktionen Sie für Ihren Mitarbeiter verwenden können. Sie können einer vorhandenen Verbindung für zukünftige Projekte zusätzliche Anwendungsfälle hinzufügen. Weitere Informationen finden Sie unter [Anwendungsfälle für die Zusammenarbeit](../overview/use-cases.md).

Um neue Anwendungsfälle hinzuzufügen, wählen Sie **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Anwendungsfälle]** aus.

![Der Bildschirm „Verbindungseinstellungen bearbeiten“, in dem der Abschnitt „Anwendungsfälle“ und die Option „Bearbeiten“ hervorgehoben sind.](/help/assets/connect/manage-connections/edit-use-cases.png){zoomable="yes"}

Aktivieren **[!UICONTROL im Dialogfeld „Anwendungsfälle]** die Option Neue Anwendungsfälle, die Sie hinzufügen möchten, gefolgt von **[!UICONTROL Speichern]**.

![Das Dialogfeld mit der hervorgehobenen Option „Speichern“.](/help/assets/connect/manage-connections/use-cases-dialog.png){zoomable="yes"}

>[!NOTE]
>
>Wenn Sie [neue Anwendungsfälle hinzufügen](#add-use-cases) z. B. „Zielgruppenaktivierung“ oder „Messung“, wird der Bildschirm „Verbindungseinstellungen bearbeiten“ aktualisiert und enthält jetzt die Abschnitte **[!UICONTROL Zielgruppenaktivierung]** und **[!UICONTROL Kreditaufteilung]**. Sie müssen die entsprechenden Einstellungen für diese neuen Anwendungsfälle konfigurieren. Weitere Informationen finden Sie in den Handbüchern [Zielgruppenaktivierung](../connect/establishing-connections.md#audience-activation) und [Kreditaufteilung](../connect/establishing-connections.md#credit-split).
>
>![Der Bildschirm „Verbindungseinstellungen bearbeiten“ mit den Abschnitten Zielgruppenaktivierung und Kreditaufteilung , nachdem neue Anwendungsfälle hinzugefügt wurden.](/help/assets/connect/manage-connections/setup-audience-activation-credit-split.png){zoomable="yes"}

### Übereinstimmungsschlüssel hinzufügen {#add-match-keys}

Für die Verbindung stehen nur Übereinstimmungsschlüssel zur Verfügung, die in Ihrem Konto konfiguriert und auch von Ihrem Mitarbeiter ausgewählt wurden. Sobald Sie [neue Übereinstimmungsschlüssel zu Ihrem Konto hinzufügen](../setup/onboard-account.md#edit-match-keys) und Ihr Mitarbeiter dieselben Schlüssel auch ausgewählt hat, können Sie diese in Ihren vorhandenen Verbindungen aktivieren.

Wählen Sie im Bildschirm „Verbindungseinstellungen bearbeiten“ **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Übereinstimmungsschlüssel]** aus.

![Der Bildschirm „Verbindungseinstellungen bearbeiten“, in dem der Abschnitt „Übereinstimmungsschlüssel“ und die Option „Bearbeiten“ hervorgehoben sind.](/help/assets/connect/manage-connections/edit-connection-match-keys.png){zoomable="yes"}

Ein **[!UICONTROL Übereinstimmungsschlüssel]** wird angezeigt, in dem die für die Verbindung konfigurierten vorhandenen Übereinstimmungsschlüssel angezeigt werden. Wählen Sie die Übereinstimmungsschlüssel aus, die Sie hinzufügen möchten, gefolgt von **[!UICONTROL Speichern]**.

![Das Dialogfeld Übereinstimmungsschlüssel mit den neu ausgewählten Übereinstimmungsschlüsseln und der Option Speichern.](/help/assets/connect/manage-connections/connection-match-keys-dialog.png){zoomable="yes"}

### Kreditaufspaltung bearbeiten {#edit-credit-split}

Die Einstellungen für die Kreditaufteilung geben an, welcher Mitarbeiter für die Kosten verantwortlich ist, die mit jedem Anwendungsfall in der Verbindung verbunden sind. Um diese Einstellungen zu aktualisieren, wählen Sie **[!UICONTROL Bearbeiten]** im Abschnitt **[!UICONTROL Kreditaufteilung]** aus.

![Der Bildschirm „Verbindungsparameter bearbeiten“, in dem der Abschnitt „Kreditaufteilung“ und die Option „Bearbeiten“ hervorgehoben sind.](/help/assets/connect/manage-connections/edit-credit-split.png){zoomable="yes"}

Wählen Sie **[!UICONTROL Dialogfeld]** Kreditaufteilung“ die bevorzugten Einstellungen für [!UICONTROL Activation-Matching] und [!UICONTROL Measurement]. Wählen Sie dann zur Bestätigung **[!UICONTROL Speichern]** aus.

![Das Dialogfeld „Kreditaufteilung“ mit den Einstellungen für die Kreditaufteilung und der Option „Speichern“.](/help/assets/connect/manage-connections/credit-split-dialog.png){zoomable="yes"}

### Änderungen überprüfen und übermitteln {#review-and-submit-changes}

Wenn Sie die Bearbeitung der Verbindungseinstellungen abgeschlossen haben, überprüfen Sie und wählen Sie **[!UICONTROL Änderungen übermitteln]**. Die Aktualisierungen der Verbindungseinstellungen werden zur Überprüfung an Ihren Mitarbeiter gesendet.

![Der Bildschirm „Verbindungseinstellungen bearbeiten“ mit den Optionen Aktualisierungen und Änderungen übermitteln.](/help/assets/connect/manage-connections/review-and-submit-changes.png){zoomable="yes"}

#### Änderungen der Verbindungseinstellungen als Entwurf speichern

Sie können die Änderungen an den Verbindungseinstellungen als Entwurf speichern und jederzeit zur Fertigstellung der Aktualisierung der Verbindungseinstellungen zurückkehren.

Um die Änderungen als Entwurf zu speichern, klicken Sie auf **[!UICONTROL Abbrechen]** neben **[!UICONTROL Änderungen übermitteln]**. Wählen Sie dann im Dialogfeld **[!UICONTROL Nicht übermittelte Änderungen]** die Option **[!UICONTROL Später fortfahren]** zur Bestätigung aus.

![Der Bildschirm „Verbindungseinstellungen bearbeiten“](/help/assets/connect/manage-connections/unsubmitted-changes-dialog.png){zoomable="yes"}

Ihre Änderungen werden jetzt als Entwurf gespeichert. Im Arbeitsbereich Verbindungseinstellungen wird eine Benachrichtigung angezeigt, die darauf hinweist, dass es nicht übermittelte Änderungen gibt. Um weitere Aktualisierungen vorzunehmen, wählen Sie **[!UICONTROL Bearbeitung fortsetzen]**.

![Eine Benachrichtigung im Arbeitsbereich „Verbindungseinstellungen“, die anzeigt, dass es nicht gesendete Änderungen gibt, die auf Überprüfung und Übermittlung warten.](/help/assets/connect/manage-connections/continue-editing-connection.png){zoomable="yes"}
