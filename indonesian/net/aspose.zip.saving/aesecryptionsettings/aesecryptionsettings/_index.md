---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: AesEcryptionSettings konstruktor. Menginisialisasi instance baru dariAesEcryptionSettings kelas.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

Menginisialisasi instance baru dari[`AesEcryptionSettings`](../) kelas.

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| password | String | Kata sandi untuk enkripsi atau dekripsi. |
| method | EncryptionMethod | Opsi algoritma yang menunjukkan ukuran blok cipher. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| NotSupportedException | *method* bukan salah satu dariAES128 ,AES192 , atauAES256. |

### Contoh

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### Lihat juga

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../aesecryptionsettings/)
* perakitan [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

Menginisialisasi instance baru dari[`AesEcryptionSettings`](../)kelas tanpa password.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| method | EncryptionMethod | Opsi algoritma yang menunjukkan ukuran blok cipher. |

### Lihat juga

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../aesecryptionsettings/)
* perakitan [Aspose.Zip](../../../)


