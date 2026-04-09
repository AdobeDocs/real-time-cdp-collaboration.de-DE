---
title: Hinzufügen und Verwalten von Messdaten
description: Erfahren Sie, wie Sie Messdaten zu Adobe Real-Time CDP Collaboration hinzufügen.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 739d31b9-3f00-477d-b6be-995c7767c6ca
source-git-commit: 42bbd17878701cfaf2cba170a9471cf5c7285796
workflow-type: tm+mt
source-wordcount: '1918'
ht-degree: 5%

---

# Hinzufügen und Verwalten von Messdaten {#add-and-manage-measurement-data}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_onboard_measurement_data"
>title="Mehr dazu"
>abstract=""

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_data_target_fields"
>title="Zielfelder"
>abstract="Platzhalter für Zielfelder von Messungen."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_data_source_fields"
>title="Quellfelder"
>abstract="Platzhalter für Quellfelder von Messungen."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_measurement_mapping_source_fields"
>title="Zuordnen von Quellfeldern"
>abstract="Platzhalter für Quellfeld-Messzuordnung."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_measurement_mapping_target_fields"
>title="Zuordnen von Zielfeldern"
>abstract="Platzhalter für Zielfeld-Messzuordnung."

{{limited-availability-release-note}}

In diesem Dokument werden die Schritte zum Hinzufügen von Kampagnenmessdaten zu Adobe Real-Time CDP Collaboration beschrieben. Publisher können mit Adobe-Teams zusammenarbeiten, um Campaign-Messdaten hochzuladen. Nach dem Hochladen und Verarbeiten dieser Daten können sowohl Publisher als auch Advertiser umfassende [Kampagnenmessberichte) &#x200B;](/help/guide/collaborate/measure.md).

## Messdaten hinzufügen {#add-measurement-data}

Als Advertiser können Sie Ihre Messdaten mit Konversionsereignissen zur Verwendung in Kampagnenmessberichten in Collaboration hochladen. Konversionsdaten umfassen in der Regel Felder wie Benutzerkennung (z. B. Hash-E-Mail- oder Geräte-IDs), Zeitstempel des Konversionsereignisses und bestimmte Details des Konversionsereignisses wie Kauf oder Anmeldung.

Um Messdaten zu beziehen, navigieren Sie im Arbeitsbereich **[!UICONTROL Setup]** zur Registerkarte **[!UICONTROL Meine Messdaten]** . Wählen Sie das Symbol zum Hinzufügen aus ![Symbol hinzufügen.](/help/assets/icons/plus.png)) und wählen Sie **[!UICONTROL Messdaten]**.

Wenn dies Ihre ersten Messdaten sind, können Sie auch die Option **[!UICONTROL Hinzufügen]** auswählen.

![Registerkarte „Meine Messdaten“ mit hervorgehobener Option „Hinzufügen“ und Option „Messdaten“.](../../assets/setup/add-manage-measurement-data/add-measurement-data.png){zoomable="yes"}

Der Bildschirm **[!UICONTROL Messdaten hinzufügen]** wird angezeigt, der eine Zusammenfassung der Schritte zur Beschaffung der Messdaten enthält. Wählen Sie **[!UICONTROL Onboarding starten]** aus.

![Der Bildschirm „Messdaten hinzufügen“ mit einer Zusammenfassung der Schritte zur Quelle der Messdaten und der hervorgehobenen Option „Onboarding starten“.](../../assets/setup/add-manage-measurement-data/add-measurement-data-screen.png){zoomable="yes"}

### Datenverbindung und Details {#data-connection-and-details}

In diesem Schritt müssen Sie Ihre Datenverbindung konfigurieren und die Details für Ihre Messdaten angeben.

#### Messdatentyp auswählen {#select-measurement-data-type}

Der Messdatentyp definiert die Art der Ereignisse, die für die Kampagnenmessung eingebracht werden. Derzeit ist der unterstützte Typ „Konversionsdaten“.

Wählen Sie **[!UICONTROL Konversionsdaten]** als Messdatentyp aus, gefolgt von **[!UICONTROL Weiter]**.

![Der Schritt „Datenverbindung und Details“, in dem der Messdatentyp und die Option „Weiter“ hervorgehoben werden.](../../assets/setup/add-manage-measurement-data/select-measurement-data-type.png){zoomable="yes"}

#### Auswählen der Datenverbindung {#select-data-connection}

Eine Datenverbindung ist die Quelle, aus der Sie Messdaten in Collaboration beziehen. Nachdem Sie Ihre erste Datenverbindung hergestellt und Ihren ersten Satz von Messdaten bezogen haben, können Sie mit derselben Datenverbindung weitere Messdaten beziehen.

Um eine Datenverbindung hinzuzufügen, wählen Sie **[!UICONTROL Neue Datenverbindung hinzufügen]** und dann **[!UICONTROL Weiter]**.

![Der Schritt Datenverbindung und Details , in dem die Option Neue Datenverbindung hinzufügen und die Option Weiter hervorgehoben werden.](../../assets/setup/add-manage-measurement-data/select-measurement-data-connection.png){zoomable="yes"}

#### Datenquelle auswählen {#select-data-source}

Wählen Sie anschließend die Quelle für Ihre Datenverbindung aus. Derzeit ist Adobe Experience Platform die einzige unterstützte Datenquelle.

Wählen Sie Ihre Datenquelle und dann **[!UICONTROL Weiter]** aus.

![Der Schritt „Datenverbindung und Details“, in dem die Adobe Experience Platform-Option und die nächste Option hervorgehoben werden.](../../assets/setup/add-manage-measurement-data/select-measurement-data-source.png){zoomable="yes"}

#### Sandbox auswählen {#select-sandbox}

Wählen Sie die Sandbox aus, die die Messdaten enthält, die Sie für Collaboration Campaign-Messberichte verwenden möchten. Wählen Sie die Sandbox aus der Liste der verfügbaren Sandboxes und dann **[!UICONTROL Weiter]** aus.

![Der Schritt „Datenverbindung und Details“, in dem die Produktions-Sandbox und die Option Weiter hervorgehoben sind.](../../assets/setup/add-manage-measurement-data/select-sandbox.png){zoomable="yes"}

#### Messdatensatz auswählen {#select-measurement-dataset}

Eine Liste der Datensätze in der ausgewählten Sandbox wird angezeigt. Wählen Sie einen Datensatz als Messdaten aus und klicken Sie dann auf **[!UICONTROL Weiter]**. Sie können die Suchoption verwenden, um den bevorzugten Datensatz zu filtern und zu finden.

![Der Schritt Datenverbindung und Details , in dem die Suchoption, der Beispielereignisdatensatz und die Option Weiter hervorgehoben werden.](../../assets/setup/add-manage-measurement-data/select-measurement-dataset.png){zoomable="yes"}

#### Name und Details angeben {#provide-name-and-details}

Geben Sie als Nächstes einen Namen und eine Beschreibung für Ihre Datenverbindung an. Diese Informationen helfen Ihnen später bei der Identifizierung der Datenverbindung.

![Der Schritt Datenverbindung und Details mit der Option, einen Namen und eine Beschreibung anzugeben.](../../assets/setup/add-manage-measurement-data/data-connection-name-details.png){zoomable="yes"}

### Zuordnung {#mapping}

Der nächste Schritt besteht darin, Felder aus Ihren Messdaten den entsprechenden Zielfeldern zuzuordnen, die in Collaboration verwendet werden. Sie können Ihren Ereignisdatensatz auch mit Attributen aus dem Echtzeit-Kundenprofil anreichern, indem Sie Join-Schlüssel zuordnen und diese Attribute zum Aufschlüsseln von Messberichten verwenden.

#### Anreichern von Ereignisdaten {#enrich-event-data}

Um Ihre Ereignisdaten anzureichern, wählen Sie die Option **[!UICONTROL Source-Feld-Zusammenführungsschlüssel]** aus.

![Der Bildschirm Zuordnung mit der hervorgehobenen Option &quot;Source-Feldverknüpfungsschlüssel“.](../../assets/setup/add-manage-measurement-data/select-source-field-join-key.png){zoomable="yes"}

Wählen Sie im Dialogfeld **[!UICONTROL Source-]**-Schlüssel das Quellfeld und dann **[!UICONTROL Auswählen]** aus.

![Das Dialogfeld &quot;Source-Feldverknüpfungsschlüssel“, in dem das Source-Feld hervorgehoben ist, und die Option „Weiter“.](../../assets/setup/add-manage-measurement-data/source-field-join-key-dialog.png){zoomable="yes"}

Wählen Sie als Nächstes die Option **[!UICONTROL Profilverbindungsschlüssel]** aus. Wählen Sie **[!UICONTROL Dialogfeld Profilverknüpfungsschlüssel]** das Profilfeld aus der Liste aus. Sie können die Suchoption verwenden, um das gewünschte Feld zu finden. Wählen Sie dann zur Bestätigung **[!UICONTROL Auswählen]** aus.

![Das Dialogfeld „Profilverknüpfungsschlüssel“, in dem der Suchschlüssel, das ausgewählte Profilfeld und die Option Weiter hervorgehoben sind.](../../assets/setup/add-manage-measurement-data/profile-join-key-dialog.png){zoomable="yes"}

#### Zuordnen von Feldern {#mapping-fields}

Um mit der Zuordnung von Quellfeldern aus Ihren Messdaten zu den Zielfeldern in Collaboration zu beginnen, wählen Sie das leere Quellfeld im Bildschirm **[!UICONTROL Zuordnung]** aus.

![Der Bildschirm „Zuordnung“ mit hervorgehobenem leerem Quellfeld.](../../assets/setup/add-manage-measurement-data/mapping-screen.png){zoomable="yes"}

Das **[!UICONTROL Quellfeld auswählen]** wird angezeigt und zeigt eine Liste der verfügbaren Quellfelder an, die unter Optionen wie **[!UICONTROL Identity-Namespace]** und **[!UICONTROL Ereignisschema]** gruppiert sind. Sie können die Suchoption verwenden, um das Quellfeld aus der Liste zu filtern und zu finden.

Wählen Sie das gewünschte Quellfeld und dann **[!UICONTROL Auswählen]** aus.

![Das Dialogfeld „Quellfeld auswählen“, in dem das Quellfeld „E-Mails“ hervorgehoben ist, und die Option „Auswählen“.](../../assets/setup/add-manage-measurement-data/select-source-field-dialog.png){zoomable="yes"}

Ordnen Sie anschließend das ausgewählte Quellfeld mithilfe des Dropdown-Menüs einem entsprechenden Zielfeld zu. Alle verfügbaren Zielfelder sind die [Übereinstimmungsschlüssel, die für Ihr Mitarbeiter-Konto konfiguriert wurden](./onboard-account.md#set-up-match-keys).

![Das Dropdown-Menü mit allen verfügbaren Zielfeldern, die dem ausgewählten Quellfeld zugeordnet werden sollen.](../../assets/setup/add-manage-measurement-data/select-target-field-dropdown.png){zoomable="yes"}

Sie können bei Bedarf Zuordnungszeilen hinzufügen oder entfernen. Wenn Sie ein nicht-gehashtes Quellfeld einem gehashten Zielfeld zuordnen müssen (z. B. das Zuordnen einer Nur-Text-E-Mail zu [!UICONTROL gehashten E-Mail]), verwenden Sie die Option **[!UICONTROL Umwandlung anwenden]**, um den erforderlichen Hash anzuwenden.

Wenn Sie fertig sind, überprüfen Sie die zugeordneten Felder und fügen Sie die Schlüssel hinzu, wenn die Anreicherung aktiviert ist. Klicken Sie dann auf **[!UICONTROL Weiter]**.

![Der Bildschirm Zuordnung mit den zugeordneten Feldern, den Join-Schlüsseln (wenn die Anreicherung aktiviert ist) und der hervorgehobenen Option „Weiter“.](../../assets/setup/add-manage-measurement-data/review-mapping.png){zoomable="yes"}

### Einverständnisverwaltung {#manage-consent}

Bevor Sie fortfahren, müssen Sie bestätigen, dass Ihre Datennutzung in Collaboration mit Ihren Real-Time CDP-Data-Governance-Richtlinien übereinstimmt. Alle Daten müssen gemäß den Einverständnisanforderungen oder anwendbaren benutzerdefinierten Einverständnisrichtlinien vorgefiltert werden, sodass keine weitere Verarbeitung erforderlich ist.

Um Ihre Bestätigung zu bestätigen, klicken Sie **[!UICONTROL Weiter]**.

![Der Bildschirm Einverständnis verwalten , für den eine Bestätigung erforderlich ist, mit der hervorgehobenen Option „Weiter“.](../../assets/setup/add-manage-measurement-data/manage-consent.png){zoomable="yes"}

Wenn Sie [Profilanreicherung während des Zuordnungsschritts aktivieren](#enrich-event-data) können Sie Einverständnisrichtlinien aus einer Liste vordefinierter Optionen konfigurieren. Dazu gehören:

* **Marketing-Aktionen**: Verwenden Sie diese Marketing-Aktionen, um zu steuern, welche Zielgruppendaten aus Experience Platform in Collaboration importiert werden sollen.
* **Einverständnisregeln**: Wählen Sie die Einverständnisregeln aus, die auf Daten angewendet werden sollen, die aus Collaboration bezogen werden.
* **Audience**: Verwenden Sie den Zielgruppenfilter, um Zielgruppenprofile zum Einverständnis ein- oder auszuschließen.


>[!NOTE]
>
>**[!UICONTROL Data Collaboration]** unterstützt Datennutzungsbeschriftungen mit C4, C5 und C9, während **[!UICONTROL Data Science]** nur C9 unterstützt. Weitere Informationen zu Datennutzungskennzeichnungen finden Sie in der Dokumentation zu Experience Platform:
>
>* [Datennutzungs-Labels – Übersicht](https://experienceleague.adobe.com/de/docs/experience-platform/data-governance/labels/overview){target="_blank"}
>* [Glossar](https://experienceleague.adobe.com/de/docs/experience-platform/data-governance/labels/reference){target="_blank"}

Wählen Sie die bevorzugten Einstellungen aus und klicken Sie dann auf **[!UICONTROL Weiter]**.

![Der Bildschirm Einverständnis verwalten zeigt die Einverständniskonfigurationsoptionen, wenn die Profilanreicherung aktiviert ist, wobei die Option Weiter hervorgehoben ist.](../../assets/setup/add-manage-measurement-data/manage-consent-configuration-options.png){zoomable="yes"}

Bevor Sie fortfahren, müssen Sie die Bedingungen im Dialogfeld **[!UICONTROL Governance-Richtlinie und Durchsetzungsaktionen]** bestätigen und akzeptieren. Aktivieren Sie das Kontrollkästchen, gefolgt von **[!UICONTROL OK]**.

![Das Dialogfeld „Governance-Richtlinie und Durchsetzungsaktionen“ mit hervorgehobenem Kontrollkästchen und hervorgehobener Option „OK“.](../../assets/setup/add-manage-measurement-data/governance-policy-enforcement-actions-dialog.png){zoomable="yes"}

#### Zielgruppenfilter {#audience-filter}

Um bestimmte Zielgruppenprofile für das Einverständnis ein- oder auszuschließen, verwenden Sie das **[!UICONTROL Zielgruppenfilter]** Dropdown-Menü. Wenn Sie diesen Filter auswählen, wird die Benutzeroberfläche aktualisiert und die Option **[!UICONTROL Zielgruppen durchsuchen]** angezeigt. Wählen Sie **[!UICONTROL Zielgruppen durchsuchen]** aus.

![Der Bildschirm Einverständnis verwalten zeigt die Option Zielgruppen durchsuchen , nachdem der Zielgruppenfilter ausgewählt wurde.](../../assets/setup/add-manage-measurement-data/browse-audiences.png){zoomable="yes"}

Das **[!UICONTROL Audiences auswählen]** wird angezeigt. Wählen Sie eine Audience aus der Liste und dann **[!UICONTROL Auswählen]** aus.

![Das Dialogfeld „Zielgruppen auswählen“, in dem die ausgewählte Zielgruppe hervorgehoben ist, und die Option „Auswählen“.](../../assets/setup/add-manage-measurement-data/select-audiences-dialog.png){zoomable="yes"}

Die ausgewählte Zielgruppe wird jetzt angezeigt, mit der Option, sie bei Bedarf zu entfernen. Überprüfen Sie Ihre Einverständniseinstellungen und klicken Sie dann auf **[!UICONTROL Weiter]**.

![Der Bildschirm „Einverständnis verwalten“, auf dem die ausgewählte Zielgruppe für das Einverständnis und die Option Weiter hervorgehoben sind.](../../assets/setup/add-manage-measurement-data/audience-for-consent.png){zoomable="yes"}

### Konversionsereignis hinzufügen {#add-conversion-event}

Definieren Sie anschließend die Konversionsereignisse, mit denen Sie die Wirkung Ihrer Kampagnen messen möchten, z. B. Site-Besuche, Registrierungen oder abgeschlossene Käufe. Sie können bis zu **3** Konversionsereignisse für die Messung angeben.

Geben Sie den Namen des Konversionsereignisses ein und wählen Sie dann im Dropdown-Menü den Konversionstyp aus.

![Der Bildschirm Konversionsereignis hinzufügen mit hervorgehobenem Dropdown-Menü „Konversionstyp“ wurde erweitert.](../../assets/setup/add-manage-measurement-data/conversion-type-dropdown.png){zoomable="yes"}

Sie können einen Wert für die Konversion eingeben oder das Feld leer lassen, wenn Sie zu diesem Zeitpunkt keinen Wert zuweisen möchten.

![Der Bildschirm Konversionsereignis hinzufügen mit hervorgehobener Option „Konversionswert“.](../../assets/setup/add-manage-measurement-data/conversion-value.png){zoomable="yes"}

Als Nächstes müssen Sie den Duplizierungsschlüssel angeben, um anzugeben, welche Zeilen in Ihrem Ereignisdatensatz zum selben zugrunde liegenden Konversionsereignis gehören (z. B. derselbe Zeitstempel während eines Anmeldevorgangs). Dadurch wird verhindert, dass dieselbe Konversion in Messberichten mehrmals gezählt wird. Wählen Sie dazu **[!UICONTROL Duplizierungsschlüssel]** aus. Suchen Sie im Dialogfeld **[!UICONTROL Duplizierungsschlüssel]** den Schlüssel, wählen Sie ihn aus und dann **[!UICONTROL Auswählen]**.

![Das Dialogfeld „Duplizierungsschlüssel“ mit der ausgewählten Taste und der Option „Auswählen“.](../../assets/setup/add-manage-measurement-data/duplication-key-dialog.png){zoomable="yes"}

Nach Angabe des Duplizierungsschlüssels können Sie bis zu **5 % Bedingungen hinzufügen** um nur relevante Zeilen aus dem Ereignisdatensatz für die Konvertierung einzuschließen. Wählen Sie alle oder eine dieser Bedingungen aus.

Wählen Sie **[!UICONTROL Bedingung hinzufügen]** und dann die Option Bedingung aus.

![Der Bildschirm Konversionsereignis hinzufügen, in dem die Option „Bedingung“ hervorgehoben wird, nachdem die Option „Bedingung hinzufügen“ ausgewählt wurde.](../../assets/setup/add-manage-measurement-data/add-condition.png){zoomable="yes"}

Suchen Sie im **[!UICONTROL Quellfeld auswählen]** ein Quellfeld für die Bedingungsregel, gefolgt von „Auswählen **[!UICONTROL und wählen Sie es]**.

![Das Dialogfeld „Quellfeld auswählen“, in dem das Feld „Ereignistyp“ und die Option „Auswählen“ hervorgehoben sind.](../../assets/setup/add-manage-measurement-data/select-condition-field.png){zoomable="yes"}

Wählen Sie im Dropdown-Menü einen logischen Operator aus und geben Sie dann den Wert für die Bedingungsregel ein.

![Der Bildschirm Konversionsereignis hinzufügen , der das Dropdown-Menü für den logischen Operator und die Option Wert hervorhebt.](../../assets/setup/add-manage-measurement-data/logic-operator-dropdown.png){zoomable="yes"}

Um ein weiteres Konversionsereignis hinzuzufügen, wählen Sie **[!UICONTROL Konversion hinzufügen]** aus. Sie können insgesamt bis zu **3** Konversionsereignisse einbeziehen. Überprüfen Sie nach Abschluss die Konvertierungskonfigurationen und wählen Sie **[!UICONTROL Weiter]** aus.

![Der Bildschirm Konversionsereignis hinzufügen mit hervorgehobenen Konversionsereigniskonfigurationen und der hervorgehobenen Option „Weiter“.](../../assets/setup/add-manage-measurement-data/add-conversion-event.png){zoomable="yes"}

### Überprüfung {#review}

Der **[!UICONTROL Review]** wird mit einer Zusammenfassung der Einstellungen der Messdaten angezeigt. Überprüfen und stellen Sie sicher, dass alle Informationen korrekt sind. Wenn Sie einen Bereich ändern müssen, verwenden Sie die Option **[!UICONTROL Bearbeiten]**.

Wählen Sie abschließend **[!UICONTROL Abschließen]**, um das Hinzufügen Ihrer Messdaten abzuschließen.

![Der Bildschirm „Überprüfung“ mit einer hervorgehobenen Zusammenfassung der Einstellungen für Messdaten und der hervorgehobenen Option „Abschließen“.](../../assets/setup/add-manage-measurement-data/review-measurement-data.png){zoomable="yes"}

Ein Bestätigungsdialogfeld bestätigt, dass Ihre Messdaten erfolgreich erstellt wurden. Sie können die neuen Konversionsereignisse, die anhand Ihrer Messdaten konfiguriert wurden, im Arbeitsbereich &quot;**[!UICONTROL Messdaten“]**.

![Mein Arbeitsbereich für Messdaten mit einer Liste der Konversionsereignisse, die aus Ihren Messdaten konfiguriert wurden.](../../assets/setup/add-manage-measurement-data/conversion-event-list.png){zoomable="yes"}

Wählen Sie in der Rasteransicht oder Tabellenansicht ein Zeilenelement oder die Option **[!UICONTROL Konversion anzeigen]** auf einer Ereigniskarte aus, um einen Überblick über ein bestimmtes Konversionsereignis zu erhalten. Es werden der Status, die Quelle und der Name der Datenverbindung des Ereignisses zusammen mit detaillierten Bedienfeldern für Folgendes angezeigt:

* **[!UICONTROL Konversionsdetails]**: Zeigt wichtige Informationen zur Konversion an, einschließlich des Typs, des zum Identifizieren eindeutiger Ereignisse verwendeten Duplizierungsschlüssels und des zugewiesenen Konversionswerts (falls angegeben).
* **[!UICONTROL Bedingungen]**: Zeigt die auf dieses Konversionsereignis angewendeten Bedingungsregeln an.

![Der Bildschirm Überblick mit den Details für ein Konversionsereignis.](../../assets/setup/add-manage-measurement-data/conversion-event-overview.png){zoomable="yes"}

## Nächste Schritte {#next-steps}

Sie haben die Beschaffung Ihrer Messdaten in Collaboration abgeschlossen. Als Advertiser können Sie jetzt Attributionsberichte erstellen, um zu untersuchen, wie Ihre Kampagnen Konversionen fördern und die Gesamtwirkung messen. Wenn Sie Publisher sind, bitten Sie Ihren Mitarbeiter, einen Attributionsbericht für Ihre Kampagnen zu erstellen. Detaillierte Anweisungen finden Sie im Handbuch [Attributionsbericht erstellen](../collaborate/measure.md#create-attribution-report) .
