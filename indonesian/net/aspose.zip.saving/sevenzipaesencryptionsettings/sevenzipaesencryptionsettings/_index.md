---
title: "SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor SevenZipAESEncryptionSettings. Menginisialisasi sebuah instance baru dari kelas SevenZipAESEncryptionSettings"
type: docs
weight: 10
url: /id/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`SevenZipAESEncryptionSettings`](../).

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| password | String | Kata sandi untuk enkripsi atau dekripsi. |

## Contoh

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Lihat Juga

* class [SevenZipAESEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`SevenZipAESEncryptionSettings`](../) dengan cipher eksternal.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sandi | SevenZipCipher | Implementasi AES khusus. |

## Contoh

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Lihat Juga

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* assembly [Aspose.Zip](../../../)


