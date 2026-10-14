---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété ArchiveSaveOptions. Obtient ou définit les paramètres de chiffrement pour l'enregistrement d'une archive ZIP existante"
type: docs
weight: 60
url: /fr/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

Obtient ou définit les paramètres de chiffrement pour l'enregistrement d'une archive ZIP existante.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## Remarques

N'utilisez pas ces options pour la composition régulière d'une archive chiffrée, utilisez [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/) à la place.

Non compatible avec [`DataDescriptorPolicy`](../datadescriptorpolicy/) ayant la valeur ForAllFileEntries

## Exemples

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### Voir aussi

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


