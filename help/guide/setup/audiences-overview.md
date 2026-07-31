---
title: Zielgruppen – Überblick
description: Erfahren Sie mehr über Audiences in Real-Time CDP Collaboration, einschließlich der Bezugsquellen für diese.
audience: admin, publisher
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 160bd29d89d1ce828476d68e917e0271d0852eb6
workflow-type: tm+mt
source-wordcount: 707
ht-degree: 3%

---

# Zielgruppen – Überblick

{{limited-availability-release-note}}

In Adobe Real-Time CDP Collaboration sind Zielgruppen Benutzergruppen oder Kundinnen bzw. Kunden, die Sie in Collaboration einbringen. Nach der Beschaffung können Sie Zielgruppen verwenden, um Überschneidungen mit Kollegen zu ermitteln, Zielgruppen zu aktivieren und die Kampagnenleistung zu messen. Je nachdem, wo Ihre Zielgruppendaten bereits gespeichert sind, können Sie Zielgruppen aus verschiedenen Quelltypen beziehen, einschließlich Adobe Experience Platform, Cloud-Speicher- und Freigabesystemen und Datei-Upload-Workflows.

## Was Sie mit Audiences tun können {#audiences-in-collaboration}

Nachdem eine Zielgruppe aus Collaboration bezogen wurde, ist sie für die Verwendung in unterstützten Collaboration-Workflows verfügbar.

Verwenden Sie Zielgruppen in Collaboration für Folgendes:

* Vergleichen Sie Ihre Zielgruppe mit den Zielgruppen Ihrer Kollegen
* Identifizieren von Überschneidungen und Chancen
* Zielgruppen aktivieren
* Messen von Ergebnissen und Kampagnenleistung
* Verwalten der Zielgruppensichtbarkeit und der zugehörigen Einstellungen

## Anpassen von Zielgruppen an Collaboration {#conceptual-diagram}

>[!NOTE]
>
> Das folgende Diagramm zeigt in allgemeiner Form, wie die Zielgruppen der Quelle in Collaboration passen und in Projekten verwendet werden.

```text
Source → Data connection → Audience → Project
                                         │
                          ┌──────────────┼──────────────┐
                          ▼              ▼              ▼
                      Discover       Activate       Measure
                                         │
                                         ▼
                                    Destination
```

## Grundbegriffe {#core-concepts}

Die folgenden Konzepte beschreiben die wichtigsten Objekte, die an Zielgruppen-Sourcing- und Collaboration-Workflows beteiligt sind.

**Quelle**\
Das System oder der Speicherort, von dem Ihre Zielgruppendaten stammen, z. B. Adobe Experience Platform, ein Cloud-Speicherort oder ein Datei-Upload.

**Datenverbindung**\
Die konfigurierte Verbindung, die Collaboration verwendet, um auf Zielgruppendaten aus einer Quelle zuzugreifen. Eine Datenverbindung enthält quellenspezifische Konfigurationsdetails wie Authentifizierung, Feldzuordnung und Planung.

**Zielgruppe**\
Eine Benutzergruppe oder Kundschaft, die aus Collaboration bezogen wurde und in Projekten verwendet werden kann.

**Verbindung**\
Die Kooperationsbeziehung zwischen Ihrer Organisation und einer anderen Organisation.

**Projekt**\
Der Arbeitsbereich, in dem Mitwirkende Zielgruppen gemeinsam für unterstützte Anwendungsfälle wie Erkennung, Aktivierung und Messung verwenden.

**Ziel**\
Die externe Plattform oder das System, an die bzw. das aktivierte Zielgruppen gesendet werden.

**Übereinstimmungsschlüssel**
Kennungen, die Collaboration verwendet, um Datensätze über Datensätze und Mitarbeiter hinweg abzugleichen. Übereinstimmungsschlüssel unterstützen Workflows wie Zielgruppenüberschneidung, Aktivierung und Messung.

## Zielgruppen-Lebenszyklus {#audience-lifecycle}

In Collaboration können Sie Zielgruppen über Datenverbindungen beschaffen, in **[!UICONTROL Setup]** verwalten und in Projekten für unterstützte Anwendungsfälle verwenden.

1. **Source-Zielgruppen**: Binden Sie Zielgruppendaten über eine Datenverbindung in Collaboration ein.
2. **Zielgruppen verwalten**: Überprüfen und verwalten Sie Zielgruppendetails, Sichtbarkeit und zugehörige Einstellungen.
3. **Verwenden von Zielgruppen in Projekten**: Verwenden Sie die Zielgruppen aus der Quelle in Projekten für unterstützte Anwendungsfälle, einschließlich **Entdecken**, **Aktivieren** und **Messen**.

Nicht jede Zielgruppe wird in jedem Anwendungsfall verwendet. Beispielsweise kann eine Zielgruppe für &quot;**&quot; bezogen und verwendet**, ohne aktiviert zu werden, oder sie kann in **Messen“** Workflows verwendet werden, ohne an ein Ziel gesendet zu werden.

Weitere Informationen zum Abrufen und Verwalten von Zielgruppen finden Sie unter [Source und Verwalten von Zielgruppen](./onboard-audiences.md). Informationen zum Verwalten von Datenverbindungen finden Sie unter [Verwalten von Datenverbindungen](./manage-data-connection.md).

## Woher die Zielgruppen kommen {#supported-sources}

Collaboration unterstützt mehrere Zielgruppen-Quelltypen. Die ausgewählte Quelle bestimmt den Einrichtungsfluss, die Voraussetzungen, Authentifizierungsanforderungen, das Datenformat, die Feldzuordnung, das Aktualisierungsverhalten und die verfügbaren Konfigurationsoptionen für die Aufnahme von Zielgruppen in Collaboration.

* Adobe Experience Platform
* Cloud-Speicher, einschließlich Amazon S3, Google Cloud-Speicher und Azure-Speicher
* Datenfreigabe-Services, einschließlich Snowflake und Databricks Delta Share
* Adobe Audience Manager
* CSV-Datei hochladen

Eine Liste der unterstützten Quellen und quellenspezifischen Setup-Schritte finden Sie unter [Quellen - Übersicht](./source-overview.md#available-sources).

## Woraus bestehen Zielgruppen? {#match-keys}

Zielgruppen in RTCDP Collaboration bestehen aus Übereinstimmungsschlüsseln. Abhängig von Ihrer Kontokonfiguration können unterstützte Übereinstimmungsschlüssel **Personen-IDs**, **Geräte-IDs** und **Partner-IDs** umfassen. Übereinstimmungsschlüssel unterstützen Workflows wie **Zielgruppenüberschneidung**, **Aktivierung** und **Messung**.

Weitere Informationen finden Sie unter [Einrichten von Übereinstimmungsschlüsseln](../setup/onboard-account.md#set-up-match-keys) und [Datenverbindungen verwalten](../setup/manage-data-connection.md#match-keys)

## Verwenden von Zielgruppen in Projekten {#audiences-in-projects}

Projekte bieten den Kontext für die Zusammenarbeit mit einer anderen Organisation. Innerhalb eines Projekts können Sie Zielgruppen für unterstützte Anwendungsfälle der Zusammenarbeit verwenden:

* **Entdecken**: Audiences vergleichen und Überschneidungseinblicke überprüfen. Siehe [Zielgruppenüberschneidung ermitteln](../collaborate/discover.md).
* **Aktivieren**: Ausgewählte Zielgruppen für die Kampagnenverwendung aktivieren. Die Aktivierung wird von der Registerkarte [!UICONTROL Aktivieren] im Projektarbeitsbereich initiiert und sendet Zielgruppen an das konfigurierte Ziel der Verbindung. Siehe [Aktivieren von Zielgruppen](../collaborate/activate.md).
* **Kennzahl**: Überprüfen Sie die mit dem Projekt verknüpften Versand- und Konversionsberichte der Kampagne. Siehe [Leistung messen](../collaborate/measure.md).

Weitere Informationen zum Erstellen und Verwalten von Projekten finden Sie unter [Erstellen und Verwalten von Projekten](../collaborate/manage-projects.md). Informationen zum Konfigurieren von Zielen finden Sie unter [Ziele - Übersicht](../destinations/overview.md).

## Nächste Schritte {#next-steps}

* [Überprüfen der verfügbaren Zielgruppenquellen](./source-overview.md)
* [Source und Verwalten von Audiences](./onboard-audiences.md)
* [Erstellen und Verwalten von Projekten](../collaborate/manage-projects.md)
* [Zielgruppenüberschneidung ermitteln](../collaborate/discover.md)
* [Zielgruppen aktivieren](../collaborate/activate.md)
* [Leistung messen](../collaborate/measure.md)
* [Ziele – Übersicht](../destinations/overview.md)
