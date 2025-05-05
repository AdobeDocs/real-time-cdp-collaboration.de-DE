---
title: Berechnung der Überschneidungszahlen und -prozentsätze
description: Erfahren Sie, wie die Anzahl der Überschneidungen und die Prozentsätze in verschiedenen Bereichen von Adobe Real-Time CDP Collaboration berechnet werden
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 23dc33af83366806f7d99161b4b713a33daeec76
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 1%

---


# Berechnung der Überschneidungszahlen und -prozentsätze

In Adobe Real-Time CDP Collaboration ist das Verständnis der Zielgruppenüberschneidung von entscheidender Bedeutung für die Optimierung Ihrer Marketing-Strategien und die Sicherstellung einer effektiven Zusammenarbeit zwischen Werbetreibenden und Publishern. In diesem Dokument wird erläutert, wie Überschneidungszahlen und -prozentsätze in verschiedenen Produktbereichen anhand von Beispieldaten berechnet werden.

## Beispieldaten - Anzahl der Identitäten

### Annahmen für Berechnungszwecke

Nehmen wir für dieses Beispiel an, dass:

* Der Werbetreibende hat drei Zielgruppen (A1, A2, A3).
* Der Publisher hat drei Zielgruppen (P1, P2, P3).
* Alle Übereinstimmungsidentitäten schließen sich gegenseitig über alle Zielgruppen hinweg aus.

>[!NOTE]
>
>In Wirklichkeit gäbe es einige Überschneidungen zwischen den Übereinstimmungsschlüssel-Identitäten jeder Zielgruppe, aber zur Einfachheit geht dieses Beispiel davon aus, dass sie in diesem Fall exklusiv sind.

### Advertiser-Zielgruppen

| Advertiser-Zielgruppen | A1 | A2 | A3 | ALLE |
|----------------------|------|------|------|------|
| Hash-E-Mail-Identitäten | 300 K | 450 K | 250 K | 1 Mio. |
| LiveRamp-ID-Identitäten | 500 K | 200 K | 700 K | 1,4 M |
| Gesamtzahl der Identitäten | 800 K | 650 K | 950 K | 2,4 M |

### Publisher-Zielgruppen

| Publisher-Zielgruppen | P1 | P2 | P3 | ALLE |
|---------------------|------|------|------|------|
| Hash-E-Mail-Identitäten | 150 K | 600 K | 550 K | 1,3 Mio. |
| LiveRamp-ID-Identitäten | 400 K | 350 K | 100.000 | 850 K |
| Gesamtzahl der Identitäten | 550 K | 950 K | 800 K | 2,3 Mio. |

## Berechnen der Überschneidungsanzahl und -prozentsätze

### Beispieldaten - Anzahl der Überschneidungen

#### Advertiser und Publisher

|                     | A1 - P1 | A2 - P2 | A3 - P3 |
|---------------------|---------|---------|---------|
| Überschneidung durch Hash-E-Mail | 100.000 | 300 K | 150 K |
| Überschneidung nach LiveRamp-ID | 200 K | 150 K | 50 K |
| Gesamtüberschneidung | 300 K | 450 K | 200 K |

#### Advertiser und Publisher - ALLE

|                     | A1 - P ALLE | A2 - P ALLE | A3 - P ALLE |
|---------------------|------------|------------|------------|
| Überschneidung durch Hash-E-Mail | 250 K | 400 K | 200 K |
| Überschneidung nach LiveRamp-ID | 350 K | 150 K | 230 K |
| Gesamtüberschneidung | 600 K | 550 K | 430 K |

#### Advertiser ALLE vs. Publisher

|                     | A ALLE - P1 | A ALLE - P2 | A ALLE - P3 |
|---------------------|------------|------------|------------|
| Überschneidung durch Hash-E-Mail | 120 KB | 530 K | 200 K |
| Überschneidung nach LiveRamp-ID | 350 K | 330 K | 50 K |
| Gesamtüberschneidung | 470 K | 860 K | 250 K |

#### Advertiser ALL vs. Publisher ALL

|                     | A ALL - P ALL |
|---------------------|---------------|
| Überschneidung durch Hash-E-Mail | 850 K |
| Überschneidung nach LiveRamp-ID | 730 K |
| Gesamtüberschneidung | 1,58 M |

## Discover-Modul

Das **[!UICONTROL Discover]**-Modul in Adobe Real-Time CDP Collaboration bietet wertvolle Einblicke in Ihre Zielgruppendaten. Durch das Verständnis von Zielgruppenüberschneidungen können Sie potenzielle Kooperationsmöglichkeiten zwischen Publishern und Advertisern identifizieren. Im Abschnitt **[!UICONTROL Zielgruppeneinblicke]** innerhalb des Moduls **[!UICONTROL Entdecken]** können Sie die Anzahl der Überschneidungen und die Prozentsätze zwischen verschiedenen Zielgruppen analysieren.

![Das Discover-Modul des Collaboration-Workflows.](/help/assets/reference/overlap-calculations/discover-module-overlap-calculations.png)

Nachfolgend finden Sie Beispielberechnungen und Formeln für verschiedene Überschneidungsszenarien.

### Alle Advertiser-Zielgruppen und alle Publisher-Zielgruppen

| Advertiser-Zielgruppen | Publisher-Zielgruppen | Anzahl der Identitäten (a) | Identitätsüberschneidungen (b) | Überschneidungsprozentsatz | Aufschlüsselung des Übereinstimmungsschlüssels | Aufschlüsselung Schlüssel der Übereinstimmung % |
|----------------------|---------------------|--------------------|----------------------------|-----------------|---------------------|-----------------------|
| ALLE | ALLE | Gesamtzahl der Identitäten ALLER Advertiser-Zielgruppen <br> Identitätsanzahl = 1 M + 1,4 M = 2,4 M | Gesamtüberschneidung zwischen ALLEN Advertiser-Zielgruppen und ALLEN Publisher-Zielgruppen für alle Übereinstimmungsschlüssel <br> Überschneidung von Identitäten = 1,58 Mio. | Prozentsatz der sich überschneidenden Identitäten über die gesamte Identitätsanzahl ALLER Advertiser-Zielgruppen <br> Überschneidung % = (B / A) * 100 = (1,58 M / 2,4 M) * 100 = 65,83 % <br> Überschneidung Prozent = 65,83 % | Überschneidende Identitäten pro Übereinstimmungsschlüssel <br> Überschneidung durch Hash-E-Mail = 850.000 <br> Überschneidung durch LiveRamp-ID = 730.000 | Prozentsatz der Überschneidung der Übereinstimmungsschlüssel gegenüber der gesamten Identitätsüberschneidung <br> Übereinstimmungsschlüssel % für Hash-E-Mail = (850K / 1,58M) * 100 = 53,8 % <br> für Liveramp-ID = (730K / 1,58M) * 100 = 46,2 % |

### Alle Advertiser-Zielgruppen und eine Publisher-Zielgruppe

| Advertiser-Zielgruppen | Publisher-Zielgruppen | Anzahl der Identitäten (a) | Identitätsüberschneidungen (b) | Überschneidungsprozentsatz | Aufschlüsselung des Übereinstimmungsschlüssels | Aufschlüsselung Schlüssel der Übereinstimmung % |
|----------------------|---------------------|--------------------|----------------------------|-----------------|---------------------|-----------------------|
| ALLE | 1 P2 | Gesamtzahl der Identitäten aller Advertiser-Zielgruppen <br> Anzahl der Identitäten = 1 M + 1,4 M = 2,4 M | Gesamtüberschneidung zwischen ALLEN Advertiser-Zielgruppen und der ausgewählten Publisher-Zielgruppe P2 für alle Übereinstimmungsschlüssel <br> Überschneidung von Identitäten = 860.000 | Prozentsatz der sich überschneidenden Identitäten über die gesamte Identitätsanzahl ALLER Advertiser-Zielgruppen <br> Überschneidung % = (B / A) * 100 = (860 K / 2,4 M) * 100 = 35,83 % <br> Überschneidung Prozent = 35,83 % | Überschneidende Identitäten pro Übereinstimmungsschlüssel <br> Überschneidung durch Hash-E-Mail = 530.000 <br> Überschneidung durch LiveRamp-ID = 330.000 | Prozentsatz der Überschneidung des Übereinstimmungsschlüssels gegenüber der gesamten Identitätsüberschneidung <br> Übereinstimmungsschlüssel % für Hash-E-Mail = (530K / 860K) * 100 = 61,62 % <br> für LiveRamp-ID = (330K / 860K) * 100 = 38,38 % |

### Eine Advertiser-Zielgruppe und alle Publisher-Zielgruppen

| Advertiser-Zielgruppen | Publisher-Zielgruppen | Anzahl der Identitäten (a) | Identitätsüberschneidungen (b) | Überschneidungsprozentsatz | Aufschlüsselung des Übereinstimmungsschlüssels | Aufschlüsselung Schlüssel der Übereinstimmung % |
|----------------------|---------------------|--------------------|----------------------------|-----------------|---------------------|-----------------------|
| 1 A1 | ALLE | Gesamtzahl der Identitäten der vom Advertiser ausgewählten Zielgruppe A1 <br> Identitätsanzahl = 300.000 + 500.000 = 800.000 | Gesamtüberschneidung zwischen der Advertiser-Zielgruppe A1 und ALLEN Publisher-Zielgruppen für alle Übereinstimmungsschlüssel <br> Überschneidung von Identitäten = 600.000 | Prozentsatz der sich überschneidenden Identitäten über die Identitätsanzahl der vom Advertiser ausgewählten Zielgruppe (A1) <br> Überschneidung % = (B / A) * 100 = (600 K / 800 K) * 100 = 75 % <br> Überschneidung Prozent = 75 % | Überschneidende Identitäten pro Übereinstimmungsschlüssel <br> Überschneidung durch Hash-E-Mail = 250.000 <br> Überschneidung durch LiveRamp-ID = 350.000 | Prozentsatz der Überschneidung des Übereinstimmungsschlüssels gegenüber der gesamten Identitätsüberschneidung <br> Übereinstimmungsschlüssel % für Hash-E-Mail = (250K / 600K) * 100 = 41,67 % <br> für LiveRamp-ID = (350K / 600K) * 100 = 58,33 % |

### Eine Advertiser- und eine Publisher-Zielgruppe

| Advertiser-Zielgruppen | Publisher-Zielgruppen | Anzahl der Identitäten (a) | Identitätsüberschneidungen (b) | Überschneidungsprozentsatz | Aufschlüsselung des Übereinstimmungsschlüssels | Aufschlüsselung Schlüssel der Übereinstimmung % |
|----------------------|---------------------|--------------------|----------------------------|-----------------|---------------------|-----------------------|
| 1 A2 | 1 P2 | Gesamtzahl der Identitäten der vom Advertiser ausgewählten Zielgruppe A2 <br> Identitätsanzahl = 450 K + 200 K = 650 K | Gesamtüberschneidung zwischen der ausgewählten Advertiser-Zielgruppe A2 und der ausgewählten Publisher-Zielgruppe P2 für alle Übereinstimmungsschlüssel <br> Überschneidung von Identitäten = 450 K | Prozentsatz der sich überschneidenden Identitäten über die Identitätsanzahl meiner ausgewählten Zielgruppe (A2) <br> Überschneidung % = (B / A) * 100 = (450K / 650K) * 100 = 69,23 % <br> Überschneidung Prozent = 69,23 % | Überschneidende Identitäten pro Übereinstimmungsschlüssel <br> Überschneidung durch Hash-E-Mail = 300.000 <br> Überschneidung durch LiveRamp-ID = 150.000 | Prozentsatz der Überschneidung des Übereinstimmungsschlüssels gegenüber der gesamten Identitätsüberschneidung <br> Übereinstimmungsschlüssel % für Hash-E-Mail = (300K / 450K) * 100 = 66,67 % <br> für LiveRamp-ID = (150K / 450K) * 100 = 33,33 % |
