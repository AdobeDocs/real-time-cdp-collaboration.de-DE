---
title: Anforderungen an die Zielverbindung
description: Überprüfen Sie die Verbindungsinformationen, die zum Konfigurieren unterstützter Ziele in Real-Time CDP Collaboration erforderlich sind.
audience: admin, publisher
source-git-commit: c84582bb81289ce761c664af7db177535ff00a00
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 1%

---

# Anforderungen an die Zielverbindung

Bevor Sie ein Ziel in Real-Time CDP Collaboration konfigurieren, rufen Sie die vom Zielanbieter benötigten Anmeldeinformationen und Verbindungsinformationen ab.

Auf dieser Seite werden die in Collaboration verfügbaren Authentifizierungsmethoden zusammengefasst. Anweisungen zum Erstellen von Anmeldeinformationen, Zuweisen von Berechtigungen, Konfigurieren des Netzwerkzugriffs oder Vorbereiten des Zielsystems finden Sie in der Dokumentation zum verknüpften Adobe Experience Platform-Ziel .

>[!NOTE]
>
>Die verknüpfte Adobe Experience Platform-Dokumentation beschreibt den standardmäßigen Ziel-Workflow. Einige Schritte, Felder oder Optionen sind beim Konfigurieren des Ziels in Real-Time CDP Collaboration möglicherweise nicht anwendbar.

## Anforderungen auf einen Blick {#requirements-at-a-glance}

| Ziel | Authentifizierungs- oder Verbindungsmethode | Vor dem Start vorbereiten | Detaillierte Anforderungen |
|---|---|---|---|
| [!DNL Amazon S3] | Zugriffsschlüssel und geheimer Schlüssel oder übernommene Rolle | AWS-Zugriffsschlüsselpaar oder IAM-Rolle ARN; Bucket- und Ordnerinformationen | [[!DNL Amazon S3] Zieldokumentation](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/amazon-s3) |
| SFTP | Passwort oder SSH-Schlüssel | Server-Domain, Port, Benutzername, Authentifizierungsdaten und Ordnerpfad | [SFTP-Zieldokumentation](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/sftp) |
| [!DNL Azure Blob Storage] | Verbindungszeichenfolge | Azure Storage-Verbindungszeichenfolge, Container und Ordnerinformationen | [[!DNL Azure Blob Storage] Zieldokumentation](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/azure-blob) |
| [!DNL Google Cloud Storage] | Zugriffsschlüssel-ID und geheimer Zugriffsschlüssel | [!DNL Google Cloud Storage] von Interoperabilitätsanmeldeinformationen, Buckets und Ordnerinformationen | [[!DNL Google Cloud Storage] Zieldokumentation](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/google-cloud-storage) |
| [!DNL Snowflake Batch] | [!DNL Snowflake] Datenfreigabe | Konto-ID, Region, Status des privaten Links und Zugriff auf private [!DNL Snowflake] | [[!DNL Snowflake Batch] Zieldokumentation](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/warehouse/snowflake-batch) |
| [!DNL Data Landing Zone] | Keine separate Authentifizierung erforderlich | Pfad des Zielordners und Voreinstellungen für die Dateiausgabe | [[!DNL Data Landing Zone] Zieldokumentation](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/data-landing-zone) |

## Connector-Hinweise {#connector-notes}

Überprüfen Sie die folgenden Connector-spezifischen Authentifizierungsmethoden und Workflow-Unterschiede, bevor Sie ein Ziel konfigurieren.

### [!DNL Amazon S3] {#amazon-s3}

Collaboration unterstützt die **[!UICONTROL Zugriffsschlüssel]** und **[!UICONTROL Assumed Role]**-Authentifizierung. Die Authentifizierung mit Zugriffsschlüssel erfordert einen Zugriffsschlüssel und einen geheimen Zugriffsschlüssel. Für die Authentifizierung mit einer angenommenen Rolle ist die ARN einer AWS IAM-Rolle erforderlich, die Adobe übernehmen kann.

Informationen zur Einrichtung von Anmeldeinformationen, Rollen und Berechtigungen finden Sie unter [Authentifizieren beim  [!DNL Amazon S3] -Ziel](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/amazon-s3#authenticate).

### SFTP {#sftp}

Collaboration unterstützt **[!UICONTROL SFTP mit Passwort]** und **[!UICONTROL SFTP mit SSH-]**. Für beide Methoden sind die Server-Domain, der Port und der Benutzername erforderlich. Der Port ist standardmäßig auf `22` eingestellt.

Informationen zu SSH-Schlüsselformat, Server, Netzwerk und Zulassungsliste finden Sie unter [SFTP-Authentifizierungsinformationen](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/sftp#authentication-information).

### [!DNL Azure Blob Storage] {#azure-blob-storage}

Collaboration authentifiziert sich mithilfe einer Verbindungszeichenfolge für das Speicherkonto bei [!DNL Azure Blob Storage].

Anweisungen zum Abrufen der Verbindungszeichenfolge und Zuweisen von Speicherberechtigungen finden Sie unter [Authentifizieren beim  [!DNL Azure Blob Storage] -Ziel](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/azure-blob#authenticate).

### [!DNL Google Cloud Storage] {#google-cloud-storage}

Collaboration erfordert eine [!DNL Google Cloud Storage] Zugriffsschlüssel-ID und einen geheimen Zugriffsschlüssel, die über [!DNL Google Cloud Storage] Interoperabilitätseinstellungen generiert werden.

Informationen zu den Anforderungen für die Erstellung von Anmeldeinformationen und für Buckets-Berechtigungen finden Sie unter [Authentifizieren beim  [!DNL Google Cloud Storage] -Ziel](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/google-cloud-storage#authenticate).

### [!DNL Snowflake Batch] {#snowflake-batch}

[!DNL Snowflake Batch] verwendet [!DNL Snowflake] Datenfreigabe, anstatt Dateien in vom Kunden verwalteten Speicher zu exportieren. In Collaboration gibt es keinen separaten Authentifizierungsschritt. Geben Sie die Snowflake-Konto-ID, die Region, den Status des privaten Links und die Kontoeigentümerbestätigung bei der Zielerstellung ein.

Informationen zu den Anforderungen an die Kontovorbereitung und die private Auflistung finden Sie unter [[!DNL Snowflake Batch] Zieldokumentation](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/warehouse/snowflake-batch).

### [!DNL Data Landing Zone] {#data-landing-zone}

[!DNL Data Landing Zone] wird von Adobe bereitgestellt und erfordert in Collaboration keinen separaten Authentifizierungsschritt. Geben Sie bei der Zielerstellung den Zielordnerpfad und die Dateiausgabeeinstellungen an.

Informationen zum Zugriff auf eine von AWS bereitgestellte [!DNL Data Landing Zone] finden Sie unter [Authentifizieren bei der von AWS bereitgestellten Data Landing Zone](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/data-landing-zone#authenticate-dlz-aws).

## Nächste Schritte {#next-steps}

Nachdem Sie die erforderlichen Verbindungsinformationen erhalten haben, [&#x200B; Sie „ein Ziel konfigurieren und verwalten](./manage-destinations.md).
