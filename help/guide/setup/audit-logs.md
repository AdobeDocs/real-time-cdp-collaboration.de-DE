---
title: Auditprotokolle
description: Erfahren Sie, wie Sie mit der Auditprotokollfunktion in Real-Time CDP Collaboration Benutzeraktivitäten und -änderungen verfolgen können.
audience: admin
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# Auditprotokolle

{{limited-availability-release-note}}

Um die Transparenz und Sichtbarkeit der im System durchgeführten Aktivitäten zu erhöhen, können Sie die Benutzeraktivität für verschiedene Services und Funktionen in Form von Audit-Protokollen in Adobe Experience Platform überprüfen. Diese Protokolle bilden einen Audit-Trail, der Ihnen bei der Fehlerbehebung in Adobe Real-Time CDP Collaboration helfen kann und Ihrem Unternehmen dabei hilft, die Richtlinien zur Unternehmensdatenverwaltung und die gesetzlichen Anforderungen effektiv zu erfüllen.

In einem Auditprotokoll wird festgehalten *wer* welche *ausgeführt* und *wann*. Jede in einem Protokoll aufgezeichnete Aktion enthält Metadaten, die den Aktionstyp, das Datum und die Uhrzeit, die E-Mail-ID des Benutzers, der die Aktion ausgeführt hat, und zusätzliche Attribute angeben, die für den Aktionstyp relevant sind.

Verwenden Sie die Auditprotokollfunktion in Collaboration, um Benutzeraktivitäten und Änderungen innerhalb der Plattform zu verfolgen. Diese Funktion ist in den Experience Platform-Audit-Service integriert und die Benutzeroberfläche für diese Funktion befindet sich in Experience Platform.

![Übersichtsbildschirm auf hoher Ebene über die Funktionalität von Auditprotokollen.](/help/assets/setup/audit-logs/audit-logs-overview.png)

Weitere Informationen zu Auditprotokollen finden Sie in der Dokumentation zu [Experience Platform-Auditprotokollen](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}.

## Zugriff auf Auditprotokolle

Sie haben zwei Möglichkeiten, auf Auditprotokolle zuzugreifen, wie in den folgenden Abschnitten beschrieben. Beide Optionen zeigen eine Liste von Audit-Protokollen an, in denen verschiedene Aktivitäten erfasst werden, die in Collaboration ausgeführt werden.

### Zugreifen auf Auditprotokolle über die Benutzeroberfläche von Collaboration

1. Navigieren Sie zur Registerkarte **[!UICONTROL Meine Aktivität]** im **[!UICONTROL Setup]**-Arbeitsbereich in Collaboration.
2. Wählen Sie den Experience Platform-Link im Text oben auf der Seite aus.

![Greifen Sie über die Registerkarte „Meine Aktivität“ in Collaboration auf Auditprotokolle zu.](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### Zugreifen auf Auditprotokolle direkt über die Benutzeroberfläche von Experience Platform

1. Navigieren Sie zu [Experience Platform](https://platform.adobe.com/) und wählen Sie **[!UICONTROL Abschnitt]** Audits“ aus dem linken Menü aus. Wenden Sie sich an die Systemadministratoren Ihres Unternehmens, um die erforderlichen Berechtigungen zu erhalten, wenn Sie keine Auditprotokolle anzeigen können.

![Zugreifen auf Auditprotokolle über Experience Platform.](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

## Auditprotokolle anzeigen und verwenden

So zeigen Sie die Auditprotokolle an:

1. Navigieren Sie zum **[!UICONTROL Audits]** in Experience Platform.
2. Verwenden Sie [Filter](#filter-audit-logs) um die Protokolle auf der Grundlage Ihrer Kriterien einzugrenzen.
3. Wählen Sie einen Protokolleintrag aus, um detaillierte Informationen anzuzeigen, einschließlich Zeitstempel, Anfrage-ID, Ressourcendetails und Aktionsstatus.

![Detailliertes Auditprotokoll](/help/assets/setup/audit-logs/filters-and-detailed-view.png)

### Erfasste Aktivitäten

Audit-Protokolle erfassen detaillierte Informationen zu Benutzeraktivitäten, darunter:

* **Zeitstempel**: Das genaue Datum und die genaue Uhrzeit der Aktion, die in einem Monat/Tag/Jahr/Stunde:minute Format AM/PM durchgeführt wurde.
* **Asset-**: Der Name der Ressource, für die die Aktion ausgeführt wurde.
* **Kategorie**: Der Typ der Ressource, für die die Aktion ausgeführt wurde.
* **Action**: Die spezifische Aktion, die ausgeführt wird, z. B. Erstellen oder Löschen.
* **Benutzer**: Die E-Mail-Adresse des Benutzers, der die Aktion ausgeführt hat.

Diese Protokolle erstellen ein umfassendes Protokoll aller Aktivitäten in Ihrer Collaboration-Instanz, das für Data Governance und die Einhaltung gesetzlicher Vorschriften nützlich ist. Weitere Informationen [Verwalten von Auditprotokollen in der Benutzeroberfläche](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui).

### Auditprotokolle filtern {#filter-audit-logs}

Die Benutzeroberfläche für Auditprotokolle bietet mehrere Filter, mit denen Sie nach bestimmten Protokollen suchen können:

* **Kategorie**: Der Typ der Ressource, für die die Aktion ausgeführt wurde, z. B. Collaboration-Instanz oder Einladen der Collaboration-Verbindung.
* **Action**: Der Typ der durchgeführten Aktion. Die verfügbaren Aktionen hängen von der ausgewählten Kategorie ab. Aktionen für die Collaboration-Instanz umfassen beispielsweise das Erstellen, Aktualisieren und Löschen.
* **Anfrage-ID**: Eine eindeutige Kennung für die Anfrage.
* **Benutzer**: Die E-Mail-Adresse des Benutzers, der die Aktion ausgeführt hat.
* **Status**: Der Status der Aktion, z. B. „Zulassen“ oder „Ablehnen“.
* **Datumsbereich**: Der Datumsbereich, für den Sie Protokolle anzeigen möchten.

Weitere Informationen [Filtern von Auditprotokollen](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs).

## Vorteile

Audit-Protokolle bieten Unternehmen, die Collaboration verwenden, mehrere Vorteile:

* **Data Governance**: Verwenden Sie Auditprotokolle, um sicherzustellen, dass alle Aktivitäten innerhalb der Plattform verfolgt und überprüfbar sind.
* **Einhaltung gesetzlicher Vorschriften**: Die Funktion bietet eine Liste der Benutzeraktivitäten, um gesetzliche Anforderungen zu erfüllen.
* **Fehlerbehebung**: Audit-Protokolle helfen bei der Identifizierung und Lösung von Problemen, indem sie detaillierte Protokolle von Benutzeraktionen bereitstellen.

## Referenz zu Kategorien und Aktionen

Die nachstehende Tabelle enthält eine Referenz aller Kategorien und Aktionen für Real-Time CDP Collaboration.

![Verfügbare Kategorien in Real-Time CDP Collaboration-Auditprotokollen hervorgehoben.](/help/assets/setup/audit-logs/available-categories.png)

| Kategorie | Aktionen | Beschreibung |
|-------------------------------|------------------------------------------|-------------|
| **[!UICONTROL Collaboration-Instanz]** | Erstellen, Aktualisieren, Löschen | Konten verwalten, einschließlich Erstellen, Aktualisieren und Löschen von Konten. Weitere Informationen finden Sie im Handbuch [Konfigurieren Ihrer Konten](/help/guide/setup/onboard-account.md). |
| **[!UICONTROL Einladung zur Collaboration-Verbindung]** | Erstellen, Aktualisieren, Löschen, Genehmigen, Ablehnen | Verwalten Sie Verbindungseinladungen, einschließlich des Erstellens, Aktualisierens, Löschens, Genehmigens und Ablehnens von Einladungen. Weitere Informationen finden Sie im Handbuch [Herstellen von Verbindungen](/help/guide/connect/establishing-connections.md) . |
| **[!UICONTROL Collaboration-Verbindung]** | Erstellen, Aktualisieren, Löschen, Genehmigen, Ablehnen, Genehmigung anfordern | Verbindungen verwalten, einschließlich Erstellen, Aktualisieren, Löschen, Genehmigen, Ablehnen und Anfordern von Genehmigungen für Verbindungen. |
| **[!UICONTROL Collaboration-Datenverbindung]** | Erstellen, Aktualisieren, Löschen | Verwalten Sie die Datenverbindungen, aus denen Sie Zielgruppen beziehen und verwalten, einschließlich Erstellen, Aktualisieren und Löschen von Datenverbindungen. Weitere Informationen finden Sie im [Verwalten von Datenverbindungen](/help/guide/setup/manage-data-connection.md). |
| **[!UICONTROL Collaboration-Datenentität]** | Erstellen, Aktualisieren, Löschen | Verwalten von Datenentitäten für Collaboration, einschließlich Erstellen, Aktualisieren und Löschen von Datenentitäten. Datenentitäten beziehen sich in diesem Kontext auf Zielgruppen. Weitere Informationen finden Sie im Handbuch [Beschaffung und Verwaltung ](/help/guide/setup/onboard-audiences.md) Zielgruppen“. |
| **[!UICONTROL Collaboration-Projekt]** | Erstellen, Aktualisieren, Löschen | Verwalten Sie Projekte in Collaboration, einschließlich Erstellen, Aktualisieren und Löschen von Projekten. Weitere Informationen finden Sie im Handbuch [Verwalten von Projekten](/help/guide/collaborate/manage-projects.md). |
| **[!UICONTROL Collaboration-Modul]** | Erstellen, Aktualisieren, Löschen | Verwalten verschiedener Module innerhalb von Projekten, einschließlich Erstellen, Aktualisieren und Löschen verschiedener Module in der Benutzeroberfläche. Beispielsweise die Möglichkeit, [Zielgruppen zu aktivieren](/help/guide/collaborate/activate.md). |

{style="table-layout:auto"}

Durch die Nutzung der Auditprotokollfunktionen können Sie eine klare und detaillierte Aufzeichnung aller Aktivitäten in Collaboration pflegen und so Transparenz und Rechenschaftspflicht sicherstellen.
