---
title: SevenZipAESEncryptionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: Inizializza una nuova istanza diSevenZipAESEncryptionSettingsaspose.zip.saving/sevenzipaesencryptionsettings classe.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings constructor

Inizializza una nuova istanza di[`SevenZipAESEncryptionSettings`](../../sevenzipaesencryptionsettings) classe.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | Password per la crittografia o la decrittazione. |

### Esempi

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Guarda anche

* class [SevenZipAESEncryptionSettings](../../sevenzipaesencryptionsettings)
* spazio dei nomi [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings)
* assemblea [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->