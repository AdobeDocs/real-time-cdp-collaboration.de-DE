---
title: Virtual Audience Access (Zuschüsse für Zielgruppen) für RMN - Beta
description: Erfahren Sie, wie Sie in Real-Time CDP Collaboration virtuelle Audiences freigeben, Audiences finden, die für Sie freigegeben sind, und Berechtigungen, Zugriffsdauer und Sperren verwalten.
badgeBeta: label="Beta" type="Informative"
source-git-commit: 5f823194a18468b9205f64853551719ae8a3752f
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 1%
---
# Zugriff auf virtuelle Zielgruppen (Zielgruppenzuweisungen) für RMN {#virtual-audience-access}

Um Zielgruppen für verbundene Partner freizugeben, verwenden Sie den Zugriff auf virtuelle Zielgruppen in [!DNL Adobe Real-Time CDP Collaboration]. Eine Zielgruppengewährung gewährt dem Partner über eine persistente Referenz Zugriff auf die gesamte Zielgruppenpopulation. Wenn Sie Zugriff gewähren, behalten Sie die Eigentümerschaft bei, und es werden keine Zielgruppendaten verschoben.

Um eine freigegebene Zielgruppe zu verwenden, suchen Sie die virtuelle Zielgruppe in Ihrem Inventar. Verwenden Sie die Zielgruppe für die Aktivierung oder Kohorten-Zielgruppenerstellung innerhalb der Gewährungsberechtigungen. Beispielsweise kann ein Retail Media Network (RMN) Advertisern Zugriff zur Erstellung und Aktivierung von Kohorten-Zielgruppen gewähren.

## Konzepte zum Zielgruppenzugriff {#audience-access-concepts}

Um zu verstehen, was Sie freigeben und wie ein Partner die Zielgruppe verwenden kann, lesen Sie die folgenden Begriffe.

| Begriff | Beschreibung |
| --- | --- |
| Anbieter | Die Organisation, die für die Zielgruppe verantwortlich ist und den Zugriff steuert. |
| Empfängerin oder Empfänger | Der verbundene Partner, der Zugriff auf die Zielgruppe erhält. |
| erteilen | Zugriff auf eine freigegebene Zielgruppe, einschließlich zulässiger Verwendungszwecke und Zugriffsdauer. |
| Virtuelle Zielgruppe | Ein persistenter Verweis auf eine anbietereigene Zielgruppe, die im Empfängerinventar verfügbar ist. |
| Gesamtbevölkerung | Freigabe, die Zugriff auf die gesamte Zielgruppenpopulation gewährt |
| Verbindungsumfang | Zugriff, der für die Verbindung zwischen Anbieter und Empfänger gilt und nicht für ein einzelnes Projekt. |

{style="table-layout:auto"}

Zum Aktivieren einer freigegebenen Zielgruppe benötigen Sie die Berechtigung Direkte Aktivierung .

Zugriff auf virtuelle Zielgruppen gilt für eine Verbindung. Die Freigabe innerhalb eines Projekts ist ein separater Workflow und fügt keine virtuellen Zielgruppen zum Empfängerinventar hinzu.

Informationen zum Aktivieren von Zielgruppen über ein vorhandenes Kooperationsprojekt finden Sie unter [Senden und Aktivieren von Zielgruppen in einem Projekt](/help/guide/collaborate/activate.md).

## Voraussetzungen {#prerequisites}

Bevor Sie den Zugriff auf virtuelle Zielgruppen gewähren oder verwenden, stellen Sie sicher, dass Sie die folgenden Anforderungen erfüllen.

* Für Zuschüsse für virtuelle Zielgruppen stellen Sie eine aktive [Verbindung mit Ihrem Mitarbeiter“ ](/help/guide/connect/establishing-connections.md).
* Wenn Sie eine Zielgruppe bereitstellen, vergewissern Sie sich, dass die Zielgruppe zur Freigabe verfügbar ist.
* Um zu überprüfen, welche Aktionen verfügbar sind, überprüfen Sie die Gewähren von Berechtigungen für Zielgruppen, die für Sie freigegeben wurden.

Das **[!UICONTROL Audiences freigeben]** zeigt die folgenden Berechtigungen an. Beide Berechtigungen sind ausgewählt und stehen nicht zur Bearbeitung zur Verfügung.

| Zielgruppen-Berechtigung | Zulässige Verwendung |
| --- | --- |
| Direkte Aktivierung | Aktivieren einer freigegebenen Zielgruppe für ein Ziel ohne Projekt, wenn die Zielgruppe die Aktivierungsanforderungen erfüllt. |
| [!UICONTROL Neue Zielgruppe erstellen] | Verwenden Sie beim Erstellen von Zielgruppen eine freigegebene Zielgruppe als Eingabe. |

{style="table-layout:auto"}

## Freigeben einer Zielgruppe {#share-an-audience}

Um einem verbundenen Partner Zugriff auf ausgewählte Zielgruppen zu gewähren, gewähren Sie Zugriff auf die gesamte Population und legen Sie die zulässigen Verwendungen und die Dauer fest. Bei Gewährung des Zugriffs werden die Zielgruppen nicht aktiviert.

Öffnen Sie zunächst den Arbeitsbereich **[!UICONTROL Verbinden]** und die Empfängerverbindung.

![Übersicht über die Provider-Verbindung im Connect-Arbeitsbereich.](../../assets/setup/virtual-audience-access/connection-overview.png)

Wählen Sie als Nächstes **[!UICONTROL Zielgruppenzugriff]** und wählen Sie die Option für Zielgruppen aus, die Sie für den Partner freigeben.

Die Option enthält den Partnernamen. Wählen Sie in diesem Beispiel **[!UICONTROL Zu FrameSix Media]** aus.

![Auf der Registerkarte Zielgruppenzugriff wird die Option Zu FrameSix-Medien auswählen und Zugriff gewähren angezeigt.](../../assets/setup/virtual-audience-access/grant-access.png)

Wählen Sie dann **[!UICONTROL Zugriff gewähren]** aus, um das Dialogfeld **[!UICONTROL Audiences freigeben]** zu öffnen.

Wählen **[!UICONTROL in &quot;]**&quot; Zielgruppen aus **[!UICONTROL Zielgruppen auswählen]** oder wählen Sie **[!UICONTROL Zielgruppen durchsuchen]** aus.

Die ausgewählten Zielgruppen werden im Dialogfeld angezeigt. Ihr Unternehmen ist weiterhin für die Zielgruppen verantwortlich und verwaltet sie.

![Auswählen oder Durchsuchen von Zielgruppen im Dialogfeld „Zielgruppen freigeben“.](../../assets/setup/virtual-audience-access/share-audiences-selection.png)

Überprüfen Sie anschließend die angezeigten Berechtigungen in **[!UICONTROL Berechtigung]**. Mit der Berechtigung zur direkten Aktivierung kann der Partner virtuelle Zielgruppen für eigene Ziele aktivieren. **[!UICONTROL Neue Zielgruppe erstellen]** ermöglicht dem Partner die Verwendung virtueller Zielgruppen zum Erstellen neuer Zielgruppen. Beide Berechtigungen sind ausgewählt und stehen nicht zur Bearbeitung zur Verfügung.

![Berechtigungen im Dialogfeld „Zielgruppen freigeben“.](../../assets/setup/virtual-audience-access/share-audiences-permission.png)

Wählen Sie dann unter „Zugriffsdauer **[!UICONTROL eine Option]** Dauer **[!UICONTROL ,]** festzulegen, wie lange der Partner Zugriff hat. Wählen Sie **[!UICONTROL Immer]** für den Zugriff ohne Ablaufdatum aus oder geben Sie ein Datum für den zeitlich begrenzten Zugriff an.

![Das Dialogfeld Audiences freigeben zeigt eine ausgewählte Audience, ausgewählte Berechtigungen und eine Dauer an, die auf „Immer“ festgelegt ist.](../../assets/setup/virtual-audience-access/share-audiences-duration.png)

Überprüfen Sie abschließend die ausgewählten Zielgruppen, Berechtigungen und die Zugriffsdauer und wählen Sie dann **[!UICONTROL Zugriff gewähren]** aus.

Auf der Registerkarte **[!UICONTROL Zielgruppenzugriff]** werden die freigegebenen Zielgruppen mit ihrem Status, ihrer Identitätsanzahl, Zugriffsdauer, Berechtigungen und Beschreibung aufgelistet.

![Auf der Registerkarte Zielgruppenzugriff werden zwei freigegebene Zielgruppen mit dem Status Aktiv , Immer Zugriff und ihren Berechtigungen aufgelistet.](../../assets/setup/virtual-audience-access/shared-audiences.png)

Die freigegebenen Zielgruppen werden auch im Empfängerinventar als virtuelle Referenzen angezeigt. Sie behalten das Eigentum. Der Empfänger kann eine Zielgruppe separat aktivieren, wenn die Gewährung die Aktivierung zulässt.

## Suchen und Verwenden freigegebener Zielgruppen {#find-and-use-shared-audiences}

Suchen Sie als Empfänger freigegebene Zielgruppen auf der Registerkarte **[!UICONTROL Zielgruppenzugriff]** der Anbieterverbindung. Verwenden Sie jede Audience innerhalb der Gewährungsberechtigungen.

### Suchen freigegebener Zielgruppen {#find-shared-audiences}

Um Zielgruppen zu finden, die von einem Anbieter freigegeben sind, und ihre Zugriffsdetails zu überprüfen, öffnen Sie die Anbieterverbindung. Öffnen Sie zunächst den **[!UICONTROL Verbinden]**-Arbeitsbereich und die Anbieterverbindung.

Wählen Sie anschließend **[!UICONTROL Zielgruppenzugriff]** und wählen Sie die Option für vom Anbieter freigegebene Zielgruppen aus.

Die Option enthält den Anbieternamen. Wählen Sie in diesem Beispiel **[!UICONTROL Von FrameSix Media]** aus.

Überprüfen Sie abschließend die freigegebenen Audiences und ihre Zugriffsdetails.

![Die Registerkarte Zielgruppenzugriff zeigt eine von FrameSix Media freigegebene Zielgruppe an. In der Tabelle sind Status, Zugriffsdauer und Berechtigungen aufgeführt.](/help/assets/setup/virtual-audience-access/virtual-audience-access-shared-with-me.png)

### Erstellen von Zielgruppen {#build-audiences}

Um eine Zielgruppe aus einer freigegebenen Zielgruppe zu erstellen, benötigen Sie **[!UICONTROL Neue Zielgruppe erstellen]** Berechtigung. Kombinieren Sie beispielsweise eine freigegebene Zielgruppe mit Ihrer eigenen Zielgruppe, um eine neue Zielgruppe zu erstellen.

Die neue Zielgruppe gehört Ihnen. Der Anbieter behält das Eigentum an der Quell-Audience.

### Freigegebene Zielgruppen aktivieren {#activate-shared-audiences}

Für die direkte Aktivierung einer virtuellen Zielgruppe müssen Sie sicherstellen, dass die Finanzhilfe diese Bedingungen erfüllt.

| Anforderung | Bedingung |
| --- | --- |
| Freigabetyp | Gesamtbevölkerung |
| Zielgruppen-Berechtigung | Sie haben die Berechtigung zur direkten Aktivierung für die Zielgruppe. |
| Gewährungsstatus | Aktiv. Der Zugriff ist unbegrenzt oder innerhalb des angegebenen Datumsbereichs. |

{style="table-layout:auto"}

Um eine geeignete Zielgruppe an ein Ziel zu senden, verwenden Sie die Seite **[!UICONTROL Aktivieren]**. Sie benötigen kein Projekt.

Weitere Informationen finden Sie unter [Zielgruppen direkt aktivieren (Beta)](/help/guide/destinations/direct-audience-activation.md).

Wenn eine Zielgruppe die Anforderungen nicht erfüllt, können Sie die Zielgruppe nicht für die direkte Aktivierung auswählen. Collaboration überprüft die Eignung bei jeder geplanten Aktivierungsausführung erneut.

## Verwalten des Zielgruppenzugriffs {#manage-audience-access}

Als Anbieter legen Sie fest, wie lange der Zugriff dauern soll. Nur Sie können die Gültigkeit der Gewährung ändern oder den Zugriff widerrufen.

### Zugriffsdauer {#access-duration}

Wählen Sie beim Erstellen der Gewährungs-ID eine Zugriffsdauer aus.

| Dauer | Verhalten |
| --- | --- |
| [!UICONTROL Immer] | Der Zugriff läuft nicht automatisch ab. Sie können die Finanzhilfe widerrufen. |
| Datumsbereich | Der Zugriff dauert für den angegebenen Datumsbereich an. Collaboration verarbeitet den Ablauf stündlich. |

{style="table-layout:auto"}

Um den Zugriff zu verlängern, legen Sie ein künftiges Ablaufdatum fest oder ändern Sie die Dauer in einen unbegrenzten Zugriff. Bei jeder Änderung wird auch eine abgelaufene Finanzhilfe reaktiviert.

### Ablaufdatum des Zugriffs {#access-expiration}

Collaboration sucht stündlich nach abgelaufenen Zuwendungen. Wenn Collaboration einen Zuschuss als abgelaufen kennzeichnet, verliert der Empfänger virtuellen Zugriff auf die Zielgruppe.

### Zugriff widerrufen {#revoke-access}

Um den virtuellen Zugriff sofort zu entfernen, widerrufen Sie die aktive oder abgelaufene Gewährung.

![Das Dialogfeld Zugriff widerrufen warnt, dass der Partner den Zugriff auf die freigegebene Zielgruppe verliert. Die Option „Zugriff widerrufen“ ist hervorgehoben.](/help/assets/setup/virtual-audience-access/revoke-virtual-access.png)

## Nächste Schritte {#next-steps}

Nachdem Sie den Zielgruppenzugriff gewährt oder erhalten haben, verwenden Sie die folgenden Handbücher, um die Aktivierung vorzubereiten oder Collaborator-Verbindungen zu verwalten.

* [Konfigurieren und Verwalten von Zielen](/help/guide/destinations/manage-destinations.md)
* [Verwalten von Collaborator-Verbindungen](/help/guide/connect/manage-connections.md)
