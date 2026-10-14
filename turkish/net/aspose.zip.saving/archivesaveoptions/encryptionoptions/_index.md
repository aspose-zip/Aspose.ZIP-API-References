---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "ArchiveSaveOptions özelliği. Mevcut ZIP arşivini kaydederken şifreleme ayarlarını alır veya ayarlar"
type: docs
weight: 60
url: /tr/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

Mevcut ZIP arşivini kaydederken şifreleme ayarlarını alır veya ayarlar.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## Açıklamalar

Şifreli arşivin normal oluşturulması için bu seçenekleri kullanmayın, bunun yerine [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/) kullanın.

ForAllFileEntries değerine sahip [`DataDescriptorPolicy`](../datadescriptorpolicy/) ile uyumlu değildir.

## Örnekler

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### Ayrıca Bakınız

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


