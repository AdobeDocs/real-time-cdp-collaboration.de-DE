---
title: 'Administratorzugriff für Collaboration-Onboarding  [!DNL Starter] '
description: Erfahren Sie, wie Sie den Administratorzugriff für Adobe Real-Time CDP Collaboration  [!DNL Starter]  die Admin Console in Adobe Experience Cloud konfigurieren.
audience: users invited to Real-Time CDP Collaboration [!DNL Starter]
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 7b5aa5e2-1238-4a0b-be20-becfe6c9e0b7
source-git-commit: db4cc34592e49254163d7db54f93238146ce72a4
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 2%

---

# Konfigurieren des Administratorzugriffs für das Onboarding von Collaboration-[!DNL Starter]

Als erster Benutzer Ihres Unternehmens, der über Collaboration [!DNL Starter] auf Adobe Experience Platform zugreift, sind Sie für die Einrichtung und Verwaltung des Zugriffs für Ihr Team verantwortlich. Sie müssen sich selbst die erforderlichen Administrator- und Benutzerberechtigungen erteilen, um in Real-Time CDP Collaboration arbeiten zu können. Lesen Sie dieses Handbuch, um zu erfahren, wie Sie den erforderlichen Zugriff in der Admin Console konfigurieren, damit Sie Berechtigungen für die Zusammenarbeit in der Benutzeroberfläche „Berechtigungen“ verwalten können.

## Voraussetzungen {#prerequisites}

Bevor Sie fortfahren, stellen Sie Folgendes sicher:

* hat die Einladung von Ihrem lizenzierten Collaboration-Partner angenommen. Weitere Informationen zu den Einladungsanforderungen finden Sie unter [Collaboration [!DNL Starter] Overview](../overview/starter-overview.md#prerequisites).
* Die Geschäftsbedingungen von Collaboration wurden geprüft und unterzeichnet.
* Sie haben Ihre Adobe-Begrüßungs-E-Mail erhalten und Ihre erstmalige Kontoerstellung abgeschlossen.

## Zugriff einrichten {#setup-access}

Wenn Ihr Adobe-Konto über den [!DNL Starter]-Workflow erstellt wird, wird Ihnen automatisch die Rolle des Systemadministrators zugewiesen. Auf diese Weise können Sie Benutzende und den Produktzugriff in der Admin Console verwalten. Sie haben jedoch noch keinen Zugriff auf **[!UICONTROL Berechtigungen]**, der erforderlich ist, um den Zugriff für Collaboration zu verwalten.

Verwenden Sie die Admin Console, um sich selbst sowohl **Produktadministratorzugriff** auf Experience Platform als auch **Benutzerzugriff** auf Experience Platform-Produkte zu gewähren und in **[!UICONTROL Berechtigungen]** zu gelangen.

Weitere Informationen zu Rollen und Produkten in Experience Cloud finden Sie in der Dokumentation [Übersicht über die Zugriffssteuerung](../permissions/overview.md) .

>[!TIP]
>
>In diesem Handbuch bezieht sich **Administrator** auf **System- und**.

### Konfigurieren des Produktadministratorzugriffs {#configure-product-admin-access}

Lesen Sie diesen Abschnitt, um sich selbst Administratorrechte zu gewähren und mit dem Einrichten des Zugriffs für Collaboration [!DNL Starter] zu beginnen.

#### Zugriff auf Admin Console {#access-admin-console}

Melden Sie sich zunächst mit Ihren Anmeldeinformationen bei [&#128279;](https://experience.adobe.com/){target="_blank"}0&rbrace;Adobe Experience Cloud&quot; an. Eine Liste Ihrer verfügbaren Produkte finden Sie im Abschnitt **[!UICONTROL Schnellzugriff]** . Wählen Sie **[!UICONTROL Admin Console]** aus.

![Adobe Experience Cloud-Homepage mit hervorgehobener Admin Console-Karte.](../../assets/setup/starter/admin-access/select-admin-console.png){zoomable="yes"}

#### Zugriff auf das Adobe Experience Platform-Produkt-Dashboard {#access-adobe-experience-platform}

Der Arbeitsbereich [Admin Console](https://adminconsole.adobe.com/) wird auf einer neuen Registerkarte geöffnet. Wählen Sie **[!UICONTROL Adobe Experience Platform]** aus der Liste **[!UICONTROL Produkte]** unter **[!UICONTROL Produkte und Services]** aus.

![Admin Console Workspace mit hervorgehobenem Adobe Experience Platform-Produkt.](../../assets/setup/starter/admin-access/admin-console-workspace.png){zoomable="yes"}

#### Produkt-Admin hinzufügen {#add-product-admin}

Navigieren Sie im Produkt **Dashboard von** Adobe Experience Platform zur Registerkarte **[!UICONTROL Admins]**. Wählen Sie dann **[!UICONTROL Admin hinzufügen]** aus.

![Produkt-Dashboard von Adobe Experience Platform mit hervorgehobener Registerkarte „Administratoren“ und hervorgehobener Option „Administrator hinzufügen“](../../assets/setup/starter/admin-access/add-admin.png){zoomable="yes"}

Geben Sie Ihre E-Mail-Adresse oder Ihren Benutzernamen **[!UICONTROL Dialogfeld]** Produktadministratoren hinzufügen“ ein und wählen Sie dann das richtige Konto aus dem Dropdown-Menü aus. Klicken Sie abschließend auf **[!UICONTROL Speichern]**.

![Das Dialogfeld „Produktadministratoren hinzufügen“ zeigt die Kontoinformationen an, und die Option „Speichern“ ist hervorgehoben.](../../assets/setup/starter/admin-access/add-product-admin.png){zoomable="yes"}

Sie sind jetzt Produkt-Administrator und können dem Produkt in der Admin Console Benutzer oder andere Administratoren hinzufügen. Gewähren Sie sich als Nächstes Benutzerzugriff auf das Experience Platform-Produkt, um in den Berechtigungen auf Funktionen zuzugreifen und diese durchzuführen.

### Konfigurieren des Benutzerzugriffs {#configure-user-access}

Um Collaboration-Berechtigungen verwalten zu können, benötigen Sie **Benutzerzugriff** auf das Produkt zusätzlich zum Administratorzugriff. Der Benutzerzugriff kann von einem System- oder Produktadministrator konfiguriert werden.

>[!TIP]
>
>Wenn Sie dem vorherigen Abschnitt folgen, sollten Sie sich bereits im Produkt-Dashboard **[!UICONTROL Adobe Experience Platform]** von Admin Console befinden. Fahren Sie von hier aus mit [sich selbst als Benutzer hinzufügen](#add-user) fort.

Führen Sie die folgenden Schritte aus, um mit der Konfiguration Ihres Benutzerzugriffs zu beginnen:

1. [Greifen Sie über die Adobe Experience Cloud-Startseite auf die Admin Console zu](#access-admin-console).
2. [Navigieren Sie zum Adobe Experience Platform-Produkt-Dashboard](#access-adobe-experience-platform).

#### Benutzer zum Produkt hinzufügen {#add-user}

Sie befinden sich jetzt im Produkt-Dashboard {**}Adobe Experience Platform.** Navigieren Sie zur Registerkarte **[!UICONTROL Benutzer]** und wählen Sie **[!UICONTROL Benutzer hinzufügen]** aus.

![Produkt-Dashboard von Adobe Experience Platform mit hervorgehobener Registerkarte „Benutzer“ und hervorgehobener Option „Benutzer hinzufügen“](../../assets/setup/starter/admin-access/add-user.png){zoomable="yes"}

Der **[!UICONTROL Benutzer zu diesem Produkt hinzufügen]** erscheint, in dem Sie aufgefordert werden, Ihren Namen, Ihre Benutzergruppe oder Ihre E-Mail-Adresse einzugeben. Füllen Sie die Werte aus und wählen Sie dann Ihr Konto aus der Dropdown-Liste aus.

![Im Dialogfeld „Benutzer zu diesem Produkt hinzufügen“ werden die Kontoinformationen und die hervorgehobene Option „Produkte“ angezeigt.](../../assets/setup/starter/admin-access/add-users-to-product.png){zoomable="yes"}

Wählen Sie als Nächstes das Symbol zum Hinzufügen ![Symbol hinzufügen](../../assets/icons/plus.png) unter **[!UICONTROL Produkte]**.

Ein Dialogfeld mit einer Liste der verfügbaren [Produktprofile](https://helpx.adobe.com/de/enterprise/using/manage-product-profiles.html) wird angezeigt. Wählen Sie **[!UICONTROL AEP-Default-All-Users]** und **[!UICONTROL Default Production All Access]** aus. Wählen Sie dann **[!UICONTROL Übernehmen]** aus.

![Das Dialogfeld „Produktprofile auswählen“ zeigt die ausgewählten Produktprofile und die hervorgehobene Option „Anwenden“ an.](../../assets/setup/starter/admin-access/select-product-profiles.png){zoomable="yes"}

Wählen Sie abschließend **[!UICONTROL Speichern]**, um das Hinzufügen neuer Benutzer zum Produkt abzuschließen.

![Dialogfeld „Benutzer zu diesem Produkt hinzufügen“ mit hervorgehobener Option „Speichern“.](../../assets/setup/starter/admin-access/save-user.png){zoomable="yes"}

Nachdem Sie Benutzerzugriff haben, navigieren Sie zurück zu [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}. Vergewissern Sie sich **[!UICONTROL dass]** Berechtigungen“ und **[!UICONTROL Real-Time CDP Collaboration]** unter &quot;**[!UICONTROL &quot; verfügbar]**.

![Adobe Experience Cloud-Startbildschirm mit sowohl Berechtigungen als auch Real-Time CDP Collaboration, die unter Schnellzugriff aufgeführt und hervorgehoben sind.](../../assets/setup/starter/admin-access/permissions-collaboration-available.png){zoomable="yes"}

>[!TIP]
>
>Wenn **[!UICONTROL Berechtigungen]** und **[!UICONTROL Real-Time CDP Collaboration]** nicht in **[!UICONTROL Schnellzugriff]** angezeigt werden, versuchen Sie, sich abzumelden und wieder anzumelden.

## Nächste Schritte {#next-steps}

Sie haben jetzt sowohl **Administratorzugriff** als auch **Benutzerzugriff**, um Berechtigungen einzugeben, mit denen Sie Rollen definieren, spezifische Berechtigungen zuweisen und den Benutzerzugriff für Collaboration-Funktionen und -Ressourcen verwalten können. Eine schrittweise Anleitung hierzu finden Sie im [Handbuch zur Berechtigungssteuerung](./starter-permission-controls.md).
