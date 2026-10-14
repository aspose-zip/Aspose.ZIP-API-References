---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ArchiveSaveOptions eigenschap. Haalt op of stelt versleutelingsinstellingen in voor het opslaan van een bestaand ZIP-archief"
type: docs
weight: 60
url: /nl/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

Haalt op of stelt versleutelingsinstellingen in voor het opslaan van een bestaand ZIP-archief.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## Opmerkingen

Gebruik deze opties niet voor de reguliere samenstelling van een versleuteld archief, gebruik in plaats daarvan [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/)

Niet compatibel met [`DataDescriptorPolicy`](../datadescriptorpolicy/) met de waarde ForAllFileEntries

## Voorbeelden

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### Zie ook

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


