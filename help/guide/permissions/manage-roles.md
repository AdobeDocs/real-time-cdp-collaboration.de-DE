---
title: Verwalten von Rollen durch Berechtigungen
description: Machen Sie sich mit allen verfügbaren Rollenressourcen vertraut, die Zugriff auf verschiedene Komponenten in der Real-Time CDP Collaboration-Benutzeroberfläche bieten.
audience: admin
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 59cf5bf2-421b-4ebc-beab-30eafb098649
source-git-commit: a7215d453021be578a32ce1af4d659845c3b8493
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 1%

---

# Verwalten von Rollen {#manage-roles}

{{limited-availability-release-note}}

Um den Benutzerzugriff auf verschiedene Komponenten der Adobe Real-Time CDP Collaboration-Benutzeroberfläche zu verwalten, kann [Administrator](./manage-user-access.md#system-admin-gain-access) Rollen definieren und zuweisen. Rollen definieren den Zugriff, den ein Administrator oder Benutzer auf [Ressourcen](https://experienceleague.adobe.com/de/docs/experience-platform/access-control/home#permissions){target="_blank"} in Ihrer Organisation hat. Dieses Handbuch enthält Informationen zu den in Real-Time CDP Collaboration bereitgestellten Standardrollen sowie zu den individuellen Berechtigungen, die Sie benutzerdefinierten Rollen zuweisen können.

Um mit der Verwaltung von Rollen zu beginnen, benötigt ein Administrator Zugriff auf das Experience Platform-Produkt. Informationen zum Abrufen des administrativen Zugriffs oder des Zugriffs auf Experience Platform finden Sie im [Benutzerzugriff verwalten](./manage-user-access.md#manage-user-access-through-permissions).

## Standardrollen {#standard-roles}

Es werden zwei Standardrollen bereitgestellt, die zwei gängige Anwendungsfälle für die Zugriffssteuerung erfüllen. Dies sind „schreibgeschützte“ Rollen, d. h. sie können nicht angepasst werden.

| Rollenname | Rollenbeschreibung | Berechtigungen |
| --- | --- | --- | 
| Collaboration-Manager | Dies ist eine Berechtigung für uneingeschränkten Zugriff, die alle 15 Berechtigungen enthält. Dadurch kann der Benutzer alle Daten lesen, erstellen und bearbeiten. Es bietet außerdem Zugriff auf die **[!UICONTROL Prod]**-Sandbox in Experience Platform, sodass Sie Zielgruppen in Real-Time CDP Collaboration importieren können. | Alles aus der unten stehenden Tabelle. |
| Collaboration-Viewer | Dies ist eine schreibgeschützte Zugriffsberechtigung. Ein Benutzer kann Daten, Aktivitäten, Verbindungen und mehr lesen und erfassen. Es bietet außerdem Zugriff auf die **[!UICONTROL Prod]**-Sandbox in Experience Platform, sodass Sie Zielgruppen in Real-Time CDP Collaboration importieren können. | Alle Leseberechtigungen aus der folgenden Tabelle. |

{style="table-layout:auto"}

## Erstellen spezifischer Zugriffsrollen {#specific-access-roles}

Es empfiehlt sich, zusätzliche Rollen zu erstellen, um den verschiedenen Benutzern unterschiedliche Zugriffsrechte zu gewähren. Beim Erstellen von Rollen können Sie verschiedene Zugriffsebenen verwalten, indem Sie bestimmte Berechtigungen innerhalb der Ressource **[!UICONTROL Zusammenarbeit]** auswählen. Informationen zum Erstellen und Verwalten von Rollen finden Sie im Handbuch [Rollen](https://experienceleague.adobe.com/de/docs/experience-platform/access-control/abac/permissions-ui/roles#create-new-role){target="_blank"} .

>[!NOTE]
> Um Zugriff auf Collaboration zu erhalten, muss eine Benutzerin bzw. ein Benutzer Zugriff auf die **[!UICONTROL Prod]**-Sandbox in Adobe Experience Platform haben. Um einem Benutzer Zugriff auf diese Sandbox zu gewähren, muss ihm eine Rolle zugewiesen werden, die die **[!UICONTROL Prod]**-Berechtigung in der Ressource **[!UICONTROL Sandboxes]** enthält.

Nachfolgend finden Sie eine Liste der verfügbaren Berechtigungen innerhalb der Ressource Zusammenarbeit:

| Berechtigung auf hoher Ebene | Beschreibung |
| --- | --- |
| Verwalten von Collaboration-Instanzen | Anzeigen, Erstellen, Aktualisieren und Löschen der Collaboration-Instanzen einer Organisation. Entdecken Sie die Instanzen für die Zusammenarbeit anderer Organisationen. |
| Collaboration-Instanzen lesen | Lesen Sie die Instanzen für die Zusammenarbeit einer Organisation und entdecken Sie die Instanzen für die Zusammenarbeit anderer Organisationen. |
| Verwalten von Verbindungseinladungen | Von Ihrem Unternehmen initiierte Verbindungseinladungen anzeigen, erstellen und löschen. Akzeptieren und Ablehnen von Verbindungseinladungen, die von anderen Organisationen initiiert wurden |
| Lesen von Verbindungseinladungen | Anzeigen von Verbindungseinladungen. |
| Collaboration-Verbindungen verwalten | Ein Mitarbeiter kann Einstellungen anzeigen, erstellen und aktualisieren sowie Verbindungen senden und löschen. |
| Collaboration-Verbindungen lesen | Verbindungen anzeigen. |
| Verwalten von Zielgruppendaten | Onboarden und Entdecken von Zielgruppen. Aktualisieren Sie öffentliche, private und benutzerdefinierte Zielgruppen und verwalten Sie die Metadateneinstellungen des Zielgruppeninventars. |
| Zielgruppendaten lesen | Lesen und Entdecken von Zielgruppen. |
| Verwalten von Messdaten | Messdaten integrieren, aktualisieren und löschen. |
| Messdaten lesen | Messdaten lesen. |
| Projekte verwalten | Anzeigen, Erstellen, Aktualisieren und Löschen von Projekten für alle Discover-, Activate- und Measurement-Aktivitäten. |
| Projekte lesen | Zeigen Sie Projekte für alle Discover-, Activate- und Measurement-Aktivitäten an. |
| Benutzeraktivitäten lesen | Benutzeraktivitäten lesen. |
| Benutzeraktivitäten exportieren | Exportieren Sie Benutzeraktivitäten. |
| Collaboration-Kreditüberwachung lesen | Kreditüberwachung auf Organisations- und Instanzebene. |

{style="table-layout:auto"}

## Nächste Schritte

Nachdem Sie Rollen erstellt haben, die den Zugriff auf Collaboration definieren, müssen Sie [die Rollen zuweisen](./manage-user-access.md#assign-a-role) Administratoren und Benutzern zuweisen. Eine vollständige Übersicht über [&#x200B; Verwaltung von Rollen finden &#x200B;](https://experienceleague.adobe.com/de/docs/experience-platform/access-control/abac/permissions-ui/permissions) im Handbuch zum Verwalten von Berechtigungen für eine Rolle .
