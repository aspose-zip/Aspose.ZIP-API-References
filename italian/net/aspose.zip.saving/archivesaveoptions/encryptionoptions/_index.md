---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Proprietà ArchiveSaveOptions. Ottiene o imposta le impostazioni di crittografia per il salvataggio di un archivio ZIP esistente"
type: docs
weight: 60
url: /it/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

Ottiene o imposta le impostazioni di crittografia per il salvataggio di un archivio ZIP esistente.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## Osservazioni

Non utilizzare queste opzioni per la composizione regolare di un archivio crittografato, usa invece [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/).

Non compatibile con [`DataDescriptorPolicy`](../datadescriptorpolicy/) con valore ForAllFileEntries

## Esempi

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### Vedi anche

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


