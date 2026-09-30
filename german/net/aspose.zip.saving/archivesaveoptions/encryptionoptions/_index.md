---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ArchiveSaveOptions-Eigenschaft. Liest oder setzt Verschlüsselungseinstellungen zum Speichern eines bestehenden ZIP-Archivs"
type: docs
weight: 60
url: /de/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

Liest oder setzt Verschlüsselungseinstellungen zum Speichern eines bestehenden ZIP-Archivs.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## Hinweise

Verwenden Sie diese Optionen nicht für die reguläre Erstellung eines verschlüsselten Archivs, verwenden Sie stattdessen [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/).

Nicht kompatibel mit [`DataDescriptorPolicy`](../datadescriptorpolicy/) mit dem Wert ForAllFileEntries

## Beispiele

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### Siehe auch

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


