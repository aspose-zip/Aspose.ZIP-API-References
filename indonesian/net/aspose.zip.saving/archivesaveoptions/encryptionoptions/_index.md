---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti ArchiveSaveOptions. Mendapatkan atau mengatur pengaturan enkripsi untuk menyimpan arsip ZIP yang ada"
type: docs
weight: 60
url: /id/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

Mendapatkan atau mengatur pengaturan enkripsi untuk menyimpan arsip ZIP yang ada.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## Catatan

Jangan gunakan opsi ini untuk komposisi biasa arsip terenkripsi, gunakan [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/) sebagai gantinya.

Tidak kompatibel dengan [`DataDescriptorPolicy`](../datadescriptorpolicy/) yang memiliki nilai ForAllFileEntries

## Contoh

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### Lihat Juga

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


