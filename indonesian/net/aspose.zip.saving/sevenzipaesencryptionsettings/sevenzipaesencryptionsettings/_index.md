---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: SevenZipAESEncryptionSettings konstruktor. Menginisialisasi instance baru dariSevenZipAESEncryptionSettings kelas.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Menginisialisasi instance baru dari[`SevenZipAESEncryptionSettings`](../) kelas.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| password | String | Kata sandi untuk enkripsi atau dekripsi. |

### Contoh

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Lihat juga

* class [SevenZipAESEncryptionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* perakitan [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Menginisialisasi instance baru dari[`SevenZipAESEncryptionSettings`](../) kelas dengan sandi eksternal.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| cipher | SevenZipCipher | Implementasi AES khusus. |

### Contoh

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Lihat juga

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* perakitan [Aspose.Zip](../../../)


