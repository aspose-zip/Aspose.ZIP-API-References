---
title: ArchiveSaveOptions.EncryptionOptions
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveSaveOptions property. Gets of sets encryption settings for saving existing zip archive
type: docs
weight: 60
url: /net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

Gets of sets encryption settings for saving existing zip archive.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## Remarks

Do not use this options for regular composition of encrypted archive, use [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/) instead.

Not compatible with [`DataDescriptorPolicy`](../datadescriptorpolicy/) having value ForAllFileEntries

## Examples

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### See Also

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


