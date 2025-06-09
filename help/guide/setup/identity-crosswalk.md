---
title: Identitäts-Crosswalks
description: Erfahren Sie alles über Identitätsübergänge in Real-Time CDP Collaboration, einschließlich der Einbindung von Identitätsübergängen aus verschiedenen Quellen und der Verwaltung von Identitätsübergängen
audience: admin, publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
hidefromtoc: true
hide: true
exl-id: a51f112d-3da7-4482-a24a-6d9f269d28d1
source-git-commit: fda414120decc0c76712616ff85b83febede53e9
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 22%

---

# Identitäts-Crosswalks

{{limited-availability-release-note}}

Erfahren Sie alles über Identitätsübergänge in Real-Time CDP Collaboration, einschließlich der Einbindung von Identitätsübergängen aus verschiedenen Quellen und der Verwaltung von Identitätsübergängen.

Identitäts-Crosswalks erleichtern die sichere und datenschutzkonforme Verknüpfung von Kundenidentitäten über mehrere Datensätze und Plattformen hinweg. Durch die Verwendung von Hash-Kennungen stellt Real-Time CDP Collaboration sicher, dass Benutzende Identitäten synchronisieren und abgleichen können, ohne personenbezogene Daten (PII) verfügbar zu machen. Dies ermöglicht eine einheitliche Sicht auf den Kunden für eine bessere Zusammenarbeit und zielgerichtete Marketing-Maßnahmen.

<!--
In Real-Time CDP Collaboration, use identity crosswalks alongside your audiences by [TODO] insert material here. 
-->


Als ersten Schritt müssen Sie Identity Crosswalks in Real-Time CDP Collaboration importieren. Informationen zum Importieren von Identity Crosswalks in Real-Time CDP Collaboration finden Sie im folgenden Abschnitt:

>[!NOTE]
>
>In der Beta-Version von Real-Time CDP Collaboration können Sie Identitäts-Crosswalks aus Ihren Datensätzen in Real-Time CDP importieren. In nachfolgenden Versionen werden weitere Optionen verfügbar sein.

## Importieren von Identity Crosswalks in Real-Time CDP Collaboration {#import-crosswalk}

Navigieren Sie zur Registerkarte **[!UICONTROL Setup]** > **[!UICONTROL Identity Crosswalks]** und wählen Sie das Symbol hinzufügen (Symbol ![Hinzufügen) aus.](/help/assets/icons/plus.png)), und wählen Sie **[!UICONTROL Identity Crosswalk]**

![Aufzeichnung, wie Sie zum Bildschirm gelangen, um Identitäts-Crosswalks hinzuzufügen](/help/assets/setup/identity-crosswalks/import-identity-crosswalk.gif)

### Crosswalk-Quelle auswählen

Wählen Sie eine Quelle aus, aus der Sie den Identity Crosswalk importieren möchten. In der ersten Version von Real-Time CDP Collaboration ist Experience Platform die einzige unterstützte Quelle für den Import von Crosswalks.

>[!TIP]
>
>Die Überleitungen, die Sie aus Experience Platform importieren, werden in Platform als *Datensätze* bezeichnet.

Nachdem Sie Experience Platform als Quelle Ihrer Überleitungen ausgewählt haben, wählen Sie die [Experience Platform-Sandbox](https://experienceleague.adobe.com/de/docs/experience-platform/sandbox/home) aus der Sie den Identity-Überlauf importieren.

![Aufzeichnung der Auswahl einer Crosswalk-Quelle](/help/assets/setup/identity-crosswalks/select-crosswalk-source.gif)

### Crosswalk auswählen

Nachdem Sie Experience Platform als Quelle für Ihre Überleitungen ausgewählt haben,

### Details angeben

Geben Sie einen Namen und eine Beschreibung für den Identity Crosswalk an, den Sie in das Produkt importieren.

### Auswählen des Zusammenführungsschlüssels {#select-join-key}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_crosswalk_join_key"
>title="Zusammenführungsschlüssel"
>abstract="Ein Zusammenführungsschlüssel ist eine eindeutige Kennung, die zum Abgleichen und Verknüpfen von Einträgen in verschiedenen Datensätzen verwendet wird. Dadurch wird sichergestellt, dass Daten aus verschiedenen Quellen präzise mit derselben Person oder Entität verknüpft werden können. Jede der Spaltenüberschriften aus dem ausgewählten Crosswalk kann als Zusammenführungsschlüssel dienen."

Ein Zusammenführungsschlüssel ist eine eindeutige Kennung, die zum Abgleichen und Verknüpfen von Einträgen in verschiedenen Datensätzen verwendet wird. Dadurch wird sichergestellt, dass Daten aus verschiedenen Quellen präzise mit derselben Person oder Entität verknüpft werden können. Durch Auswahl des entsprechenden Join-Schlüssels können Sie Daten effektiv zusammenführen und abstimmen und so die Genauigkeit und Vollständigkeit Ihrer Kampagnen verbessern.

Jede der Spaltenüberschriften aus dem ausgewählten Crosswalk kann als Zusammenführungsschlüssel dienen.

Wählen Sie den gewünschten Join-Schlüssel für die Crosswalk-Tabelle aus und klicken Sie **[!UICONTROL Weiter]**, um mit dem nächsten Schritt fortzufahren.

### Überprüfung

Überprüfen Sie eine der Auswahlen in den vorherigen Bildschirmen. Wenn Sie mit Ihrer Auswahl zufrieden sind, klicken Sie auf **[!UICONTROL Weiter]**, um den Workflow abzuschließen.

## Nächste Schritte

Nachdem Sie gelernt haben, wie Sie Identitäts-Crosswalks in Real-Time CDP importieren, können Sie sich alle Identitäts-Crosswalks ansehen, die Sie bisher zu Real-Time CDP Collaboration hinzugefügt haben. Sie können jetzt auch die Identity-Überleitungen verwenden, die Sie beim Importieren von Zielgruppen in Real-Time CDP Collaboration importiert haben.
