---
title: Auditprotokolle
description: Erfahren Sie, wie Sie mit der Auditprotokollfunktion in Real-Time CDP Collaboration Benutzeraktivitäten und -änderungen verfolgen können.
audience: admin
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
source-git-commit: ff22dde9730fab89481338753b1dc4a0adf1d57e
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 1%

---

# Auditprotokolle

{{limited-availability-release-note}}

Um die Transparenz und Sichtbarkeit der im System durchgeführten Aktivitäten zu erhöhen, können Sie die Benutzeraktivität für verschiedene Services und Funktionen in Form von Audit-Protokollen in Adobe Real-Time Customer Data Platform (CDP) überprüfen. Diese Protokolle bilden einen Audit-Trail, der Ihnen bei der Fehlerbehebung in Real-Time CDP Collaboration helfen kann und Ihrem Unternehmen dabei hilft, die Richtlinien zur Unternehmensdatenverwaltung und die gesetzlichen Anforderungen effektiv zu erfüllen.

In einem Auditprotokoll wird festgehalten *wer* welche *ausgeführt* und *wann*. Jede in einem Protokoll aufgezeichnete Aktion enthält Metadaten, die den Aktionstyp, das Datum und die Uhrzeit, die E-Mail-ID des Benutzers, der die Aktion ausgeführt hat, und zusätzliche Attribute angeben, die für den Aktionstyp relevant sind.

Verwenden Sie die Auditprotokollfunktion in Real-Time CDP Collaboration, um Benutzeraktivitäten und Änderungen innerhalb der Plattform zu verfolgen. Diese Funktion ist in den Adobe Experience Platform-Audit-Service integriert und die Benutzeroberfläche für diese Funktion befindet sich in Experience Platform.

![Übersichtsbildschirm auf hoher Ebene über die Funktionalität der Auditprotokolle](/help/assets/setup/audit-logs/audit-logs-overview.png)

Weitere Informationen zu Auditprotokollen finden Sie in der Dokumentation zu [Adobe Experience Platform-Auditprotokollen](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}.

## Zugriff auf Auditprotokolle

Sie haben zwei Möglichkeiten, auf Auditprotokolle zuzugreifen, wie in den folgenden Abschnitten beschrieben. Beide Optionen zeigen eine Liste von Audit-Protokollen an, in denen verschiedene Aktivitäten erfasst werden, die in der Benutzeroberfläche von Real-Time CDP Collaboration ausgeführt werden

### Zugreifen auf Auditprotokolle über die Benutzeroberfläche von Real-Time CDP Collaboration

1. Real-Time CDP Collaboration Navigieren Sie in der Benutzeroberfläche von **[!UICONTROL zur]** „Meine Aktivität .
2. Wählen Sie den Experience Platform-Link im Text der Benutzeroberfläche oben auf der Seite aus.

![Zugreifen auf Auditprotokolle über die Real-Time CDP Collaboration-Benutzeroberfläche](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### Zugreifen auf Auditprotokolle direkt über die Benutzeroberfläche von Experience Platform

1. Navigieren Sie zur Adobe Experience Platform-Benutzeroberfläche und wählen Sie **[!UICONTROL Abschnitt]** Audits“ aus dem linken Menü aus. Wenden Sie sich an die Systemadministratoren Ihres Unternehmens, um die erforderlichen Berechtigungen zu erhalten, wenn Sie keine Auditprotokolle anzeigen können.

![Zugreifen auf Auditprotokolle über die Experience Platform-Benutzeroberfläche](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

## Auditprotokolle anzeigen und verwenden

So zeigen Sie die Auditprotokolle an:

1. Navigieren Sie zum **[!UICONTROL Audits]** in der Adobe Experience Platform-Benutzeroberfläche.
2. Verwenden Sie die Filter, um die Protokolle auf der Grundlage Ihrer Kriterien einzugrenzen.
3. Wählen Sie einen Protokolleintrag aus, um detaillierte Informationen anzuzeigen, einschließlich Zeitstempel, Anfrage-ID, Ressourcendetails und Aktionsstatus.

![Detailliertes Auditprotokoll](/help/assets/setup/audit-logs/filters-and-detailed-view.png)

### Erfasste Aktivitäten

Audit-Protokolle erfassen detaillierte Informationen zu Benutzeraktivitäten, darunter:

* **Benutzer-ID**: Die Kennung des Benutzers, der die Aktion ausgeführt hat.
* **Action**: Der Typ der durchgeführten Aktion (z. B. Erstellen, Aktualisieren, Löschen).
* **Ressource**: Die Ressource, die geändert oder erstellt wurde.
* **Zeitstempel**: Der Zeitpunkt, zu dem die Aktion ausgeführt wurde.

Diese Protokolle erstellen ein umfassendes Protokoll aller Aktivitäten in Ihrer Real-Time CDP Collaboration-Instanz, das für Data Governance und die Einhaltung gesetzlicher Vorschriften nützlich ist. Weitere Informationen [Verwalten von Auditprotokollen in der Benutzeroberfläche](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui).

### Auditprotokolle filtern

Die Benutzeroberfläche für Auditprotokolle bietet mehrere Filter, mit denen Sie nach bestimmten Protokollen suchen können:

* **Kategorie**: Bezieht sich auf den Ressourcentyp (z. B.: Kooperationsinstanz, Verbindung, Projekt).
* **Action**: Der Typ der durchgeführten Aktion (z. B.: Erstellen, Löschen, Aktualisieren).
* **Anfrage-ID**: Eine eindeutige Kennung für die Anfrage.
* **Benutzer-E** Mail: Die E-Mail-Adresse des Benutzers, der die Aktion ausgeführt hat.
* **Status**: Der Status der Aktion (z. B.: zulässig, verweigert).
* **Datumsbereich**: Der Datumsbereich, für den Sie Protokolle anzeigen möchten.

Weitere Informationen [Filtern von Auditprotokollen](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs).

### Anwendungsbeispiel

Auditprotokolle werden in der Experience Platform-Audits-Benutzeroberfläche generiert und angezeigt, wenn Sie in der Real-Time CDP Collaboration-Benutzeroberfläche Aktionen durchführen, z. B. Zielgruppen verwalten, Verbindungseinladungen erweitern, Projekte erstellen usw. Beispielsweise werden Vorgänge zum Erstellen oder Aktualisieren von Teilen eines Projekts wie unten dargestellt erfasst:

![Beispiel für Audit-Protokolle, die beim Erstellen und Aktualisieren von Teilen eines Projekts generiert wurden.](/help/assets/setup/audit-logs/create-project-audits.png)

## Vorteile

Verstehen Sie einige Vorteile der Verwendung von Audit-Protokollen:

* **Data Governance**: Verwenden Sie Auditprotokolle, um sicherzustellen, dass alle Aktivitäten innerhalb der Plattform verfolgt und überprüfbar sind.
* **Einhaltung gesetzlicher Vorschriften**: Die Funktion bietet eine Liste der Benutzeraktivitäten, um gesetzliche Anforderungen zu erfüllen.
* **Fehlerbehebung**: Audit-Protokolle helfen bei der Identifizierung und Lösung von Problemen, indem sie detaillierte Protokolle von Benutzeraktionen bereitstellen.

## Referenz zu Kategorien und Aktionen

Die nachstehende Tabelle enthält eine Referenz aller Kategorien und Aktionen für Real-Time CDP Collaboration.

![Verfügbare Kategorien in Real-Time CDP Collaboration-Auditprotokollen hervorgehoben.](/help/assets/setup/audit-logs/available-categories.png)

| Kategorie | Aktionen | Beschreibung |
|-------------------------------|------------------------------------------|-------------|
| **[!UICONTROL Collaboration-Instanz]** | Erstellen, Aktualisieren, Löschen | Verwalten Sie Organisationskonten, einschließlich Erstellen, Aktualisieren und Löschen von Organisationen. Weitere Informationen über [Einrichten von Organisationen](/help/guide/setup/onboard-organization.md). |
| **[!UICONTROL Einladung zur Collaboration-Verbindung]** | Erstellen, Aktualisieren, Löschen, Genehmigen, Ablehnen | Verwalten Sie Verbindungseinladungen, einschließlich des Erstellens, Aktualisierens, Löschens, Genehmigens und Ablehnens von Einladungen. Lesen Sie mehr über [Verbindungseinladungen](/help/guide/connect/establishing-connections.md). |
| **[!UICONTROL Collaboration-Verbindung]** | Erstellen, Aktualisieren, Löschen, Genehmigen, Ablehnen, Genehmigung anfordern | Verwalten Sie Zusammenarbeitsverbindungen, einschließlich Erstellen, Aktualisieren, Löschen, Genehmigen, Ablehnen und Anfordern von Genehmigungen für Verbindungen. |
| **[!UICONTROL Collaboration-Datenverbindung]** | Erstellen, Aktualisieren, Löschen | Verwalten Sie Datenverbindungen für die Zusammenarbeit, um Zielgruppen zu importieren und zu verwalten, einschließlich Erstellen, Aktualisieren und Löschen von Datenverbindungen. Weitere Informationen [Verwalten von Datenverbindungen](/help/guide/setup/manage-data-connection.md). |
| **[!UICONTROL Collaboration-Datenentität]** | Erstellen, Aktualisieren, Löschen | Verwalten Sie Datenentitäten für die Zusammenarbeit, einschließlich Erstellen, Aktualisieren und Löschen von Datenentitäten. Datenentitäten beziehen sich in diesem Kontext auf Zielgruppen. Weitere Informationen über [Importieren und Verwalten von Audiences](/help/guide/setup/onboard-audiences.md). |
| **[!UICONTROL Collaboration-Projekt]** | Erstellen, Aktualisieren, Löschen | Verwalten Sie Projekte in Zusammenarbeit, einschließlich Erstellen, Aktualisieren und Löschen von Projekten. Weitere Informationen über [Verwalten von Projekten](/help/guide/collaborate/manage-projects.md). |
| **[!UICONTROL Collaboration-Modul]** | Erstellen, Aktualisieren, Löschen | Verwalten Sie verschiedene Module innerhalb von Kollaborationsprojekten, einschließlich Erstellen, Aktualisieren und Löschen verschiedener Module in der Benutzeroberfläche. Beispielsweise die Möglichkeit, [Audiences freizugeben](/help/guide/collaborate/share.md). |

{style="table-layout:auto"}

Durch die Nutzung der Auditprotokollfunktionen können Sie eine klare und detaillierte Aufzeichnung aller Aktivitäten in Ihrer Real-Time CDP Collaboration-Instanz aufbewahren, um Transparenz und Rechenschaftspflicht sicherzustellen.
