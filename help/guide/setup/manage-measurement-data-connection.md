---
title: Verwalten von Messdatenverbindungen
description: Erfahren Sie, wie Sie Messdatenverbindungen verwalten, einschließlich Details und Übereinstimmungsschlüsseln in Real-Time CDP Collaboration
audience: administrator, data engineer
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 494277f421606eda62b74c254f1fdd29b22e3473
workflow-type: tm+mt
source-wordcount: '1338'
ht-degree: 3%

---

# Verwalten von Messdatenverbindungen

{{limited-availability-release-note}}

## Überblick

Verwenden Sie Messdatenverbindungen in Real-Time CDP Collaboration, um Ihre Konversionsdaten von verschiedenen Plattformen zu beziehen. Erfahren Sie, wie Sie Details verwalten und Schlüssel für Ihre vorhandenen Datenverbindungen abgleichen.

## Anzeigen von Messdatenverbindungen {#view-measurement-data-connections}

Sie können Details zu jeder vorhandenen Messdatenverbindung anzeigen, einschließlich der Quelle Ihrer Konversionsdaten, der verwendeten Übereinstimmungsschlüssel und aller mit der Verbindung verknüpften Konversionsereignisse.

Navigieren Sie im **[!UICONTROL Setup]**-Arbeitsbereich zur Registerkarte **[!UICONTROL Meine Datenverbindungen]** . Alle aktuellen Messdatenverbindungen werden im Abschnitt **[!UICONTROL Messung]** in der Tabellen- oder Rasteransicht angezeigt. Wählen Sie **[!UICONTROL Datenverbindung anzeigen]** auf der entsprechenden Verbindungskarte aus oder wählen Sie den Datenverbindungsnamen aus, wenn Sie sich in der Tabellenansicht befinden, um den zugehörigen Arbeitsbereich zu öffnen und alle Details anzuzeigen.

![Die Registerkarte „Meine Datenverbindungen“, auf der eine Messdatenverbindungskarte hervorgehoben ist, und die Option „Datenverbindung anzeigen“.](/help/assets/setup/manage-measurement-data-connection/view-measurement-data-connection.png){zoomable="yes"}

### Verbindungsdetails für Messdaten {#measurement-data-connection-details}

In diesem Abschnitt werden die folgenden Details der Datenverbindung angezeigt:

| Feld | Beschreibung |
|-------------------|-------------|
| Status | Der aktuelle Status der Messdatenverbindung, z. B. **[!UICONTROL Aktiv]**. |
| Quelle | Die Plattform oder das System, die/das die Messdaten für diese Verbindung bereitstellt. |
| Sandbox | Der Name der Sandbox, in der die Messdatenverbindung konfiguriert ist. |
| Datensatz | Der Name des Datensatzes, der für die Beschaffung von Messdaten in der Verbindung verwendet wird. |
| Zuletzt aktualisiert | Der Zeitstempel der letzten Aktualisierung der Messdatenverbindung. |
| Zuletzt aktualisiert von | Der Benutzer, der die Messdatenverbindung zuletzt geändert hat. |
| Erstellt | Der Zeitstempel, zu dem die Messdatenverbindung erstellt wurde. |
| Erstellt von | Der Benutzer, der ursprünglich die Messdatenverbindung erstellt hat. |

{style="table-layout:auto"}

### Übereinstimmungsschlüssel {#match-keys}

Übereinstimmungsschlüssel sind die Zielfelder, denen Sie Ihre Quellfelder zugeordnet haben, wenn [&#x200B; Ihre Messdaten beziehen](./onboard-measurement-data.md). Weitere Informationen zur Funktionsweise von Übereinstimmungsschlüsseln finden Sie im Handbuch [Übereinstimmungsschlüssel](./onboard-account.md#set-up-match-keys) .

![Ein Arbeitsbereich für die Messdatenverbindung mit hervorgehobenem Abschnitt „Übereinstimmungsschlüssel“.](/help/assets/setup/manage-measurement-data-connection/view-match-keys.png){zoomable="yes"}

### Konversionsereignisse {#conversion-events}

Unten im Arbeitsbereich wird eine Liste der Konversionsereignisse angezeigt, die an die Datenverbindung angehängt sind. Die Liste zeigt einen kurzen Überblick über jedes Ereignis an, einschließlich Status, Konvertierungstyp und Quelle. Sie können den Ereignisnamen auswählen, um die Konfigurationen anzuzeigen und zu bearbeiten, oder das Konversionsereignis mit der Löschoption entfernen (![Löschsymbol](/help/assets/common/delete.svg)). Eine vollständige Anleitung zum Verwalten eines Konversionsereignisses finden Sie im Handbuch [Hinzufügen und Verwalten von &#x200B;](./onboard-measurement-data.md)&quot;.

![Ein Arbeitsbereich für die Messdatenverbindung mit hervorgehobenem Abschnitt „Konversionsereignisse“.](/help/assets/setup/manage-measurement-data-connection/view-conversion-events.png){zoomable="yes"}

## Messdatenverbindung bearbeiten {#edit-measurement-data-connection}

Sie können die Details und Übereinstimmungsschlüssel einer vorhandenen Messdatenverbindung jederzeit aktualisieren, um sicherzustellen, dass Ihre Berichte und Analysen korrekt bleiben. Navigieren Sie zunächst zur Registerkarte **[!UICONTROL Meine Datenverbindungen]** und wählen Sie die Messdatenverbindung aus, die Sie bearbeiten möchten. Dadurch wird der Arbeitsbereich Datenverbindung geöffnet, in dem Sie die folgenden Schritte ausführen können, um die erforderlichen Änderungen vorzunehmen.

### Name und Beschreibung bearbeiten {#edit-name-and-description}

Um den Namen und die Beschreibung der Datenverbindung zu aktualisieren, klicken Sie auf das Bearbeitungssymbol (![Bearbeiten](/help/assets/icons/edit.png)) neben dem Namen der aktuellen Verbindung.

![Der Arbeitsbereich für die Messdatenverbindung, in dem das Symbol „Bearbeiten“ neben dem Namen der Datenverbindung hervorgehoben ist.](/help/assets/setup/manage-measurement-data-connection/edit-name-description.png){zoomable="yes"}

Aktualisieren **[!UICONTROL im Dialogfeld „Datenverbindung bearbeiten]** die Felder mit den gewünschten Werten und wählen Sie dann **[!UICONTROL Speichern]**, um Ihre Änderungen anzuwenden.

![Das Dialogfeld „Datenverbindung bearbeiten“ mit hervorgehobener Option „Speichern“.](/help/assets/setup/manage-measurement-data-connection/edit-name-description-dialog.png){zoomable="yes"}

Es wird ein Bestätigungsdialogfeld angezeigt, das bestätigt, dass die Details erfolgreich aktualisiert wurden.

### Übereinstimmungsschlüssel bearbeiten {#edit-match-keys}

>[!IMPORTANT]
>
>Beachten Sie Folgendes, bevor Sie die Übereinstimmungsschlüssel für eine Datenverbindung bearbeiten:
>
>* Für Datenverbindungen können nur Übereinstimmungsschlüssel verwendet werden, die für Ihr Konto konfiguriert sind.
>* Derzeit können Sie zusätzliche Übereinstimmungsschlüssel zu einer Datenverbindung hinzufügen, aber sobald ein Übereinstimmungsschlüssel aktiviert ist, kann er nicht mehr entfernt werden.

Wählen Sie im Arbeitsbereich Datenverbindung die Option **[!UICONTROL Bearbeiten]** im Bedienfeld **[!UICONTROL Übereinstimmungsschlüssel]** aus.

![Der Abschnitt „Übereinstimmungsschlüssel“ mit hervorgehobener Option „Bearbeiten“.](/help/assets/setup/manage-measurement-data-connection/edit-match-keys.png){zoomable="yes"}

Es wird ein Bestätigungsdialogfeld angezeigt, in dem erklärt wird, dass alle Änderungen an der Datenverbindung für alle zugehörigen Konvertierungen gelten. Klicken **[!UICONTROL zur]** auf OK. Sie können diese Bestätigung später überspringen.

![Bestätigungsdialogfeld, das anzeigt, dass alle Änderungen an der Datenverbindung für alle zugehörigen Konvertierungen gelten.](/help/assets/setup/manage-measurement-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

Im Dialogfeld **[!UICONTROL Übereinstimmungsschlüssel]** können Sie die Anreicherungseinstellungen überprüfen und die aktuellen Zuordnungen zwischen Ihren Quellfeldern und den Zielfeldern (Übereinstimmungsschlüssel) sehen.

![Das Dialogfeld Schlüssel abgleichen mit den Anreicherungseinstellungen und vorhandenen Zuordnungen zwischen Quellfeldern und den entsprechenden Zielfeldern.](/help/assets/setup/manage-measurement-data-connection/edit-match-keys-dialog.png){zoomable="yes"}

#### Anreicherung {#enrichment}

Wenn die Anreicherung beim [&#x200B; Ihrer Messdaten nicht aktiviert &#x200B;](./onboard-measurement-data.md), haben Sie die Möglichkeit, Ihren Ereignisdatensatz mit Attributen aus dem Echtzeit-Kundenprofil anzureichern. Beachten Sie, dass die Anreicherung für Messdaten nicht mehr deaktiviert werden kann, sobald sie aktiviert wurde. Sie können die Join-Schlüssel der Anreicherung weiterhin nach Bedarf aktualisieren.

Wenn Sie die Anreicherung im Dialogfeld **[!UICONTROL Übereinstimmungsschlüssel]** aktivieren, wird die Benutzeroberfläche erweitert, um weitere Konfigurationsoptionen unter dem Abschnitt **[!UICONTROL Anreichern Ihrer Ereignisdaten mit IDs aus Profilen]** anzuzeigen.

Wählen Sie die Option **[!UICONTROL Source-]**-Schlüssel.

![Das Dialogfeld „Schlüssel abgleichen“ mit hervorgehobener Option &quot;Source-Feldverknüpfungsschlüssel“.](../../assets/setup/manage-measurement-data-connection/enrich-event-data.png){zoomable="yes"}

Wählen Sie im Dialogfeld **[!UICONTROL Source-]**-Schlüssel das Quellfeld und dann **[!UICONTROL Auswählen]** aus.

![Das Dialogfeld &quot;Source-Feldverknüpfungsschlüssel“, in dem das ausgewählte Quellfeld und die Option Weiter hervorgehoben sind.](../../assets/setup/manage-measurement-data-connection/source-field-join-key-dialog.png){zoomable="yes"}

Wählen Sie als Nächstes die Option **[!UICONTROL Profilverbindungsschlüssel]** aus. Wählen Sie **[!UICONTROL Dialogfeld Profilverknüpfungsschlüssel]** das Profilfeld aus der Liste aus. Sie können die Suchoption verwenden, um das gewünschte Feld zu finden. Wählen Sie dann zur Bestätigung **[!UICONTROL Auswählen]** aus.

![Das Dialogfeld „Profilverknüpfungsschlüssel“, in dem das ausgewählte Profilfeld und die Option „Auswählen“ hervorgehoben sind.](../../assets/setup/manage-measurement-data-connection/profile-join-key-dialog.png){zoomable="yes"}

#### Mapping bearbeiten {#edit-mapping}

Um einen vorhandenen Übereinstimmungsschlüssel zu bearbeiten, aktualisieren Sie sein verknüpftes Quellfeld und Zielfeld im Dialogfeld **[!UICONTROL Übereinstimmungsschlüssel]**. Wenn Sie einen neuen Übereinstimmungsschlüssel einbeziehen möchten, wählen Sie **[!UICONTROL Feld hinzufügen]** aus. Dadurch wird eine leere Zeile erstellt, in der Sie eine zusätzliche Zuordnung zwischen Quell- und Zielfeldern definieren können.

![Nach Auswahl von Feld hinzufügen zeigt das Dialogfeld Übereinstimmungsschlüssel eine leere neue Zuordnungszeile an, die eingegeben werden kann.](/help/assets/setup/manage-measurement-data-connection/add-new-field.png){zoomable="yes"}

Wählen Sie anschließend das leere Quellfeld aus. Das Dialogfeld **[!UICONTROL Quellfeld auswählen]** wird mit einer Liste der verfügbaren Quellfelder angezeigt, die unter Optionen wie **[!UICONTROL Identity-]** und **[!UICONTROL Profilattribute]** gruppiert sind. Sie können die Liste filtern und das gewünschte Quellfeld mit der Suchoption finden.

Wählen Sie das gewünschte Quellfeld und dann **[!UICONTROL Auswählen]** aus.

![Das Dialogfeld „Quellfeld auswählen“, in dem die Suchoption, das Telefonquellenfeld und die Option „Auswählen“ hervorgehoben sind.](/help/assets/setup/manage-measurement-data-connection/select-source-field.png){zoomable="yes"}

Verwenden **[!UICONTROL im Dialogfeld]**&#x200B;Übereinstimmungsschlüssel“ das Dropdown-Menü, um das neue Quellfeld einem Zielfeld zuzuordnen. Alle verfügbaren Zielfelder sind die für Ihr Mitarbeiter-Konto konfigurierten Übereinstimmungsschlüssel. Wenn das gewünschte Zielfeld nicht angezeigt wird, fügen Sie [die Übereinstimmungsschlüssel Ihres Kontos bearbeiten](./onboard-account.md#edit-match-keys) hinzu.

Verwenden Sie die Option **[!UICONTROL Umwandlung anwenden]**, wenn Sie ein nicht gehashtes Feld für ein gehashtes Zielfeld verwenden möchten, z. B. wenn Sie dem Zielfeld **[!UICONTROL gehashtes Telefon]** ein reines Telefonquellenfeld zuordnen.

![Das Dropdown-Menü mit allen verfügbaren Zielfeldern, die dem neuen Quellfeld zugeordnet werden sollen.](/help/assets/setup/manage-measurement-data-connection/target-field-dropdown.png){zoomable="yes"}

Nachdem Sie die Zuordnungsfelder abgeschlossen haben, überprüfen Sie Ihre Aktualisierungen und wählen Sie **[!UICONTROL Bestätigen]**, um die Änderungen anzuwenden.

![Das Dialogfeld „Übereinstimmungsschlüssel“, das die aktualisierte Feldzuordnung mit hervorgehobener Option „Bestätigen“ anzeigt.](/help/assets/setup/manage-measurement-data-connection/confirm-edit-match-keys.png){zoomable="yes"}

Ein Bestätigungsdialogfeld bestätigt, dass die Übereinstimmungsschlüssel erfolgreich aktualisiert wurden.

## Datenverbindung löschen

Durch das Löschen einer Datenverbindung werden alle zugrunde liegenden Konversionen, zugehörigen Einstellungen und die Verwendung in Collaboration entfernt. Diese Aktion kann nicht rückgängig gemacht werden.

Um eine vorhandene Datenverbindung zu löschen, wählen Sie das Löschsymbol (![Löschsymbol) &#x200B;](/help/assets/common/delete.svg) Arbeitsbereich einer einzelnen Datenverbindung aus.

![Ein Arbeitsbereich für Datenverbindungen mit hervorgehobener Löschoption.](/help/assets/setup/manage-measurement-data-connection/delete-measurement-data-connection.png){zoomable="yes"}

Ein Bestätigungsdialogfeld wird angezeigt. Wählen Sie **[!UICONTROL Löschen]** aus, um das Löschen der Datenverbindung abzuschließen.

![Das Dialogfeld „Datenverbindung löschen“ mit hervorgehobener Option „Löschen“.](/help/assets/setup/manage-measurement-data-connection/delete-measurement-data-connection-confirm.png){zoomable="yes"}

Ein Bestätigungsdialogfeld bestätigt, dass die Datenverbindung erfolgreich gelöscht wurde.

## Nächste Schritte {#next-steps}

Nach der Verwaltung Ihrer Messdatenverbindungen haben Sie folgende Möglichkeiten:

* Fügen Sie bei Bedarf weitere Konversionsereignisse hinzu, die mit Ihrer Datenverbindung verknüpft sind. Ausführliche Anweisungen finden Sie in der Dokumentation [Hinzufügen und Verwalten von &#x200B;](./onboard-measurement-data.md)&quot;.
* Erzeugen von Messberichten, um Einblicke in die Leistung und Wirkung Ihrer Kampagne zu erhalten. Weitere Informationen zu den verfügbaren Berichtstypen und deren Erstellung finden Sie im Handbuch [Leistung messen](/help/guide/collaborate/measure.md) .
