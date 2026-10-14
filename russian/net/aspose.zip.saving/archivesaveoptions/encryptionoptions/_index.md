---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство ArchiveSaveOptions. Получает или задает параметры шифрования для сохранения существующего ZIP‑архива"
type: docs
weight: 60
url: /ru/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

Получает или задает настройки шифрования для сохранения существующего ZIP‑архива.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## Примечания

Не используйте эти параметры для обычного создания зашифрованного архива, вместо этого используйте [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/).

Не совместимо с [`DataDescriptorPolicy`](../datadescriptorpolicy/) со значением ForAllFileEntries

## Примеры

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### См. также

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


