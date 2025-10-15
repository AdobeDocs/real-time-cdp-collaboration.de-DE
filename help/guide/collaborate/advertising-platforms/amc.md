---
title: Amazon Marketing Cloud
description: Erfahren Sie mehr über die Zusammenarbeit mit Amazon Marketing Cloud in Real-Time CDP Collaboration.
audience: publisher, advertiser
badgelimitedavailability: label="Eingeschränkte Verfügbarkeit" type="Informative" url="https://helpx.adobe.com/de/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 57b847c25edbf88f4708bda74be41fe6141472a7
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 20%

---

# Amazon Marketing Cloud

{{limited-availability-release-note}}

Nachdem Sie eine Verbindung mit [!DNL Amazon Marketing Cloud] ([!DNL AMC]) hergestellt haben, können Advertiser [ein Projekt erstellen](../manage-projects.md#create-project) um mit [!DNL AMC] zusammenzuarbeiten und so die erweiterten Analysefunktionen von zu nutzen. Nachdem Sie ein Projekt erstellt haben, können Sie den Abschnitt **[!UICONTROL Entdecken]** verwenden, um Zielgruppeneinblicke zu vergleichen und relevante Zielgruppen für Ihre Kampagnen zu ermitteln.

>[!IMPORTANT]
>
>Die einzigen von [!DNL AMC] unterstützten Anwendungsfälle sind **Zielgruppenerkennung** und **Messung**. Derzeit ist in Ihrem Projekt **[!UICONTROL nur der]** „Entdecken“ mit [!DNL AMC] verfügbar.

## Entdecken {#discover}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_compare_audiences"
>title="Vergleichen von Zielgruppen"
>abstract="Vergleichen Sie Ihre Zielgruppe mit allen Verbrauchenden, die von Ihren Amazon Ads erreicht werden."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_relevant_audiences"
>title="Relevante Zielgruppen"
>abstract="Targeting-Segmente in Amazon, mit denen Ihre Zielgruppe die größten Überschneidungen aufweist, wobei nur DSP-Impressions berücksichtigt werden (diese Segmente können nur in der DSP angesprochen werden)."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_resolved_ids"
>title="Aufgelöste IDs"
>abstract="Die Anzahl der IDs, die die Identitätsauflösung von Amazon mithilfe Ihrer Zielgruppendaten auflösen konnte."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlapping_ad_exposed_ids"
>title="Überlappende IDs, die Anzeigen sehen"
>abstract="Dies stellt die Anzahl der IDs unter „Aufgelöste IDs“ aus der hochgeladenen Zielgruppe dar, die ebenfalls über Amazon Ads eine Anzeige gesehen haben."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlap_percentage"
>title="Überschneidung in %"
>abstract="Der Anteil der IDs unter „Aufgelöste IDs“, die über Amazon Ads eine Anzeige gesehen haben."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_amazon_breakdown"
>title="Aufschlüsselung nach Amazon Ad-Produkt"
>abstract="Die Aufschlüsselung der IDs unter „Überlappende IDs, die Anzeigen sehen“ erfolgt entweder über Amazon Ads Sponsored Product und/oder über Amazon Ads DSP."

Im Abschnitt **[!UICONTROL Entdecken]** können Sie Ihre AMC-Zielgruppe mit allen Verbrauchern vergleichen, die von Ihren Amazon-Anzeigen erreicht werden. Sie können auch Zielgruppensegmente für Amazon anzeigen, mit denen Ihre Zielgruppe die größten Überschneidungen aufweist, wobei nur DSP-Impressions berücksichtigt werden (diese Segmente können nur in der DSP angesprochen werden).

>[!IMPORTANT]
>
>Zielgruppendaten werden aus den Zielgruppen verarbeitet, die in Ihr [!DNL Amazon Ads]-Konto hochgeladen wurden. Um zu erfahren, wie Sie mit der Funktion „Ziele“ von Experience Platform Ihre Zielgruppen an Ihr [!DNL Amazon Ads]-Konto senden können, lesen Sie das Handbuch [Amazon Ads-Verbindung](https://experienceleague.adobe.com/de/docs/experience-platform/destinations/catalog/advertising/amazon-ads).

![Der Abschnitt „Entdecken“ in einem Projekt mit Amazon Marketing Cloud.](/help/assets/collaborate/advertising-platforms/amc-discover.png){zoomable="yes"}

### Vergleichen von Zielgruppen {#compare-audiences}

Der Abschnitt **[!UICONTROL Zielgruppen vergleichen]** bietet Einblicke in die Überschneidung Ihrer [!DNL AMC] Zielgruppe mit den von Ihren Amazon-Anzeigen erreichten Verbrauchern. Im Abschnitt **[!UICONTROL Audiences vergleichen]** können Sie die folgenden Metriken anzeigen:

| Metrik | Beschreibung |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL Aufgelöste IDs] | Die Anzahl der IDs, die [!DNL Amazon’s Identity Resolution] mithilfe Ihrer Zielgruppendaten auflösen konnte. |
| [!UICONTROL Überlappende Anzeigen-offen gelegte IDs] | Die Anzahl [!UICONTROL aufgelösten IDs] aus der hochgeladenen Zielgruppe, die auch einer Anzeige über [!DNL Amazon Ads] bereitgestellt wurden. |
| [!UICONTROL Überschneidung %] | Der Anteil der [!UICONTROL aufgelösten IDs], die über [!DNL Amazon Ads] einer Anzeige bereitgestellt wurden. |
| [!UICONTROL Aufschlüsselung nach Amazon-Anzeigenprodukt] | Aufschlüsselung der [!UICONTROL sich überschneidenden und offen gelegten IDs], erreicht entweder [!UICONTROL Sponsored Product] und/oder [!UICONTROL DSP]. Jeder wird als einzelner Prozentsatz der Gesamtzahl der angezeigten Werbe-IDs dargestellt. Da eine ID sowohl zu [!UICONTROL gesponserten Produkten] als auch zu [!UICONTROL DSP] gehören kann, dürfen sich die Prozentsätze nicht auf 100 % summieren. |


### Relevante Zielgruppen {#relevant-audiences}

Der Abschnitt **[!UICONTROL Relevante Zielgruppen]** bietet Einblicke in [!DNL Amazon] Targeting-Segmente oder -Zielgruppen, mit denen Ihre Zielgruppe die größten Überschneidungen aufweist, wobei nur DSP-Impressions berücksichtigt werden (diese Segmente können nur in der DSP angesprochen werden). Sie können alle relevanten Zielgruppen umschalten. Innerhalb jedes Abschnitts können Sie die folgenden Metriken anzeigen:

| Metrik | Beschreibung |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL Aufgelöste IDs] | Die Anzahl der IDs, die [!DNL Amazon’s Identity Resolution] mithilfe Ihrer Zielgruppendaten auflösen konnte. |
| [!UICONTROL Überlappende Anzeigen-offen gelegte IDs] | Dies stellt die Anzahl der [!UICONTROL aufgelösten IDs] aus der hochgeladenen Zielgruppe dar, die auch einer Anzeige über [!DNL Amazon Ads] bereitgestellt wurden. Hierbei werden nur DSP-Impressions berücksichtigt. |
| [!UICONTROL Überschneidung %] | Der Anteil der [!UICONTROL aufgelösten IDs], die über [!DNL Amazon Ads] einer Anzeige bereitgestellt wurden. |
| [!UICONTROL Kategorien] | Die Kategorie(n), zu der die Zielgruppe gehört. Eine Zielgruppe kann mehreren Kategorien angehören. |

### Entdecken Sie Überschneidungen mit [!DNL Amazon Marketing Cloud] {#discover-overlaps}

Der Abschnitt **[!UICONTROL Entdecken Sie Überschneidungen mit Amazon Marketing Cloud]** bietet Einblicke in die Überschneidung Ihrer Zielgruppen mit [!DNL Amazon] Zielgruppensegmenten oder Zielgruppen. Sie können die folgenden Metriken anzeigen:

| Metrik | Beschreibung |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL Aufgelöste IDs] | Die Anzahl der IDs, die [!DNL Amazon’s Identity Resolution] mithilfe Ihrer Zielgruppendaten auflösen konnte. |
| [!UICONTROL Überlappende Anzeigen-offen gelegte IDs] | Dies stellt die Anzahl der [!UICONTROL aufgelösten IDs] aus der hochgeladenen Zielgruppe dar, die auch einer Anzeige über [!DNL Amazon Ads] bereitgestellt wurden. Hierbei werden nur DSP-Impressions berücksichtigt. |
| [!UICONTROL Überschneidung %] | Der Anteil der [!UICONTROL aufgelösten IDs], die über [!DNL Amazon Ads] einer Anzeige bereitgestellt wurden. |