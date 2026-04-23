---
title: RTCDP Collaboration - Starter - Übersicht
description: Erfahren Sie, wie Sie mit Adobe Real-Time CDP Collaboration Starter die datenschutzorientierte Zusammenarbeit mit einem lizenzierten Partner erweitern und verbessern können, ohne eine eigene vollständige Real-Time CDP-Lizenz zu benötigen.
audience: publisher, advertiser, invited users to Real-Time CDP Collaboration Starter
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 7ae0bd3d-eee9-48c0-9f18-a56033fee52d
source-git-commit: 3d29985d88e6370b4a0e8cd3d56358e85bb91e06
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 3%

---

# Übersicht über Adobe Real-Time CDP Collaboration [!DNL Starter]

Verwenden Sie Adobe Real-Time CDP Collaboration [!DNL Starter], um mit einem lizenzierten Partner an datenschutzorientierten Datenprojekten zusammenzuarbeiten. Sie benötigen keine eigene Collaboration-Lizenz, um teilzunehmen.

Ihr Lizenzpartner lädt Sie zu Collaboration ein und finanziert mit seinen Credits Ihre gemeinsamen Workflows, und zwar sowohl zwischen Werbekunden als auch zwischen Marken. Weitere Informationen zu diesen Mustern und ihrer Funktionsweise finden Sie in den Handbüchern [Zusammenarbeitsmuster](./collaboration-patterns.md) und [End-to-End-Workflow](./end-to-end-workflow.md).

Als eingeladener [!DNL Starter] können Sie:

* Onboarden und Verwalten von Kooperationsdaten in einem [!DNL Starter].
* Source und pflegen Zielgruppen zur Verwendung in gemeinsamen Projekten.
* Gewinnen Sie Einblicke in Zielgruppenüberschneidungen mit Ihrem Partner, um effektives Targeting und Kampagnenmessung zu unterstützen.
* Zielgruppen aktivieren und für die gemeinsame Kampagnenaktivierung und -interaktion an Ihren Partner zurückgeben.

## Voraussetzungen {#prerequisites}

Stellen Sie für die ersten Schritte mit Collaboration [!DNL Starter] sicher, dass sich sowohl Ihr Unternehmen als auch Ihr lizenzierter Partner in derselben Region befinden. Sie müssen von einem Partner eingeladen werden, der über eine Real-Time CDP Prime-, Ultimate- oder Collaboration-Lizenz verfügt.

Geben Sie Ihrem lizenzierten Partner die folgenden Informationen, um die Einladung einzuleiten:

* Contact name
* Kontakt-E-Mail
* Firma
* Rolle (Advertiser/Publisher): Advertiser
* Branche

Nachdem Sie die Einladung erhalten und angenommen haben, muss Ihr Unternehmen einen kostenlosen Kundenauftrag mit Adobe prüfen und unterzeichnen, um auf Collaboration [!DNL Starter] zugreifen zu können. Weitere Informationen zum Einladungsprozess finden Sie im Handbuch [Einladen eines Mitarbeiters zu Collaboration [!DNL Starter]](../connect/establishing-connections.md#invite-collaborator-to-starter).

## Leitlinien {#guardrails}

In der folgenden Tabelle finden Sie die wichtigsten Leitplanken für Ihr [!DNL Starter]. Dazu gehören Beschränkungen in Bezug auf Zielgruppen-Sourcing, Datenvolumen, Aktualisierungshäufigkeit, Zielgruppenüberschneidungen und Aktivierungsfunktionen.

| Leitplanke | Beschreibung |
|----------| ------------|
| Zielgruppenquelle | Sie können Zielgruppendaten mit **[!DNL Amazon S3]** als Quelle in Collaboration importieren. For step-by-step instructions, see [how to configure [!DNL Amazon S3] for audience sourcing](../setup/configure-aws-s3-audience-sourcing.md). |
| Zielgruppe | Ihr [!DNL Starter]-Konto hat maximal Anspruch auf:<ul><li>10 Zielgruppen aus einem [!DNL AWS S3] Bucket</li><li>50 Millionen Identitäten insgesamt (berechnet durch die Anzahl der Zeilen in Ihren Zielgruppendaten)</li><li>1 Aktualisierung pro Zielgruppe alle 6 Tage</li></ul> |
| Zielgruppenüberschneidungen und Einblicke | Es gibt keine Nutzungsbeschränkung dafür, wie oft Sie Zielgruppenüberschneidungen und Einblicke in Ihren Zielgruppen ausführen können. Erfahren Sie, wie Sie [Überschneidungen erkennen und Zielgruppen vergleichen](../collaborate/discover.md). |
| Activation | Als [!DNL Starter] können Sie Zielgruppen nur für den Partner aktivieren und freigeben, der Sie eingeladen hat. Die Konfiguration von Zielen für externe Plattformen ist nicht verfügbar. Weitere Informationen über [Aktivieren von Audiences](../collaborate/activate.md). |

{style="table-layout:auto"}

## Erste Schritte {#getting-started}

Nachdem Sie [ Einladung angenommen und den Bedingungen zugestimmt haben](../connect/establishing-connections.md#accept-invitation-sign-terms) melden Sie sich mit Ihren Anmeldeinformationen bei ](https://experience.adobe.com/){target="_blank"}2}Adobe Experience Cloud an. [Bevor Sie Collaboration verwenden können, müssen Sie Ihrem Konto den entsprechenden Zugriff und die entsprechenden Rollen gewähren.

Verwenden Sie diesen Workflow, um Ihr [!DNL Starter] Konto einzurichten und mit Ihrem Partner zusammenzuarbeiten.

### Einrichten des Administratorzugriffs {#setup-admin-access}

Verwenden Sie zunächst den Arbeitsbereich **Admin-Zugriff**, um sich selbst den erforderlichen Zugriff zu gewähren. Dadurch wird sichergestellt, dass Sie sowohl über Administratorrechte als auch über Benutzerzugriff auf Experience Platform-Produkte verfügen. Ausführliche Anweisungen zum Einrichten des Erstzugriffs finden Sie unter [Administratorzugriffsanweisungen](../setup/starter-admin-access.md).

Nach Abschluss des Vorgangs sollten **[!UICONTROL Berechtigungen]**, **[!UICONTROL Experience Platform]** und **[!UICONTROL Real-Time CDP Collaboration]** im Abschnitt **[!UICONTROL Schnellzugriff]** auf Ihrer [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}-Homepage angezeigt werden.

![Der Adobe Experience Cloud-Arbeitsbereich mit Berechtigungen, Experience Platform und Real-Time CDP Collaboration nach dem Einrichten des Produktadministratorzugriffs.](/help/assets/overview/starter/setup-admin-access.png){zoomable="yes"}

Weitere Informationen zu Zugriffsrollen und verschiedenen Adobe Experience Cloud-Produkten finden Sie unter [Zugriffssteuerung - Übersicht](../permissions/overview.md).

### Berechtigungen konfigurieren {#configure-permissions}

Nachdem Sie nun über Administratorrechte verfügen, können Sie sich selbst und anderen Benutzern in Ihrem Unternehmen Rollen und Berechtigungen zuweisen. Dieser Schritt ist erforderlich, bevor Sie auf Real-Time CDP Collaboration zugreifen oder anderen die Verwendung erlauben können. Detaillierte Anweisungen finden Sie unter [Konfigurieren von Berechtigungen](../setup/starter-permission-controls.md). Weitere Informationen zu den verschiedenen in Collaboration verfügbaren Rollen und Berechtigungen finden Sie in der Dokumentation [Rollen verwalten](../permissions/manage-roles.md) .

Nachdem Sie die Rollen und Berechtigungen zugewiesen haben, vergewissern Sie sich, dass Sie auf Collaboration zugreifen können. Navigieren Sie zu [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"} und wählen Sie **[!UICONTROL Real-Time CDP Collaboration]** im Abschnitt **[!UICONTROL Schnellzugriff]** aus. Dadurch wird der Arbeitsbereich **[!UICONTROL Adobe Real-Time CDP Collaboration]** geöffnet, in dem Sie mit der Verwendung von Collaboration-Funktionen beginnen können.

### Verbindungen einrichten {#set-up-connections}

Führen Sie anschließend die in den folgenden Handbüchern beschriebenen Schritte aus, um eine Verbindung herzustellen und mit Ihrem Partner zusammenzuarbeiten:

* [Einrichten des Collaboration-Kontos](../setup/onboard-account.md)
* [Herstellen einer Verbindung mit Ihrem einladenden Mitarbeiter](../connect/overview.md)
* [Erstellen Sie ein neues Projekt und beginnen Sie die Zusammenarbeit mit Ihrem Partner](../collaborate/overview.md)

### Verwendung von Guthaben verstehen {#understand-credit-usage}

Für alle Collaboration [!DNL Starter]-Aktivitäten werden Guthaben verwendet. Als eingeladener Benutzer müssen Sie diese Credits jedoch nicht erwerben oder verwalten. Der Mitarbeiter, der Sie eingeladen hat, deckt die gesamte Kreditnutzung ab, die mit Ihren Aktivitäten verbunden ist. Weitere Informationen finden Sie in der [Dokumentation zu Kreditnutzung und -nutzung in Collaboration [!DNL Starter]](../setup/starter-credit-usage.md).

## Nächste Schritte {#next-steps}

Sie haben jetzt die Ersteinrichtung abgeschlossen und Ihr Unternehmen für eine sichere Zusammenarbeit konfiguriert. Als Nächstes sehen Sie sich die folgenden Ressourcen an, um mehr über die Beschaffung von Audiences und verschiedene Projektanwendungsfälle in Collaboration zu erfahren:

* [Source und Verwalten von Audiences](../setup/onboard-audiences.md)
* [Projektanwendungsfälle](../collaborate/overview.md#project-use-cases):
   * [Überschneidungen erkennen und Zielgruppen vergleichen](../collaborate/discover.md)
   * [Zielgruppen aktivieren](../collaborate/activate.md)
   * [Kampagnenleistung messen](../collaborate/measure.md)
