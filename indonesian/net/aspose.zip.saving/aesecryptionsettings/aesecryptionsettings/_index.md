---
title: "AesEcryptionSettings.AesEcryptionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor AesEcryptionSettings. Menginisialisasi sebuah instance baru dari kelas AesEcryptionSettings."
type: docs
weight: 10
url: /id/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`AesEcryptionSettings`](../).

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| password | String | Kata sandi untuk enkripsi atau dekripsi. |
| metode | EncryptionMethod | Opsi algoritma yang menunjukkan ukuran blok cipher. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| NotSupportedException | *method* bukan salah satu dari AES128, AES192, atau AES256. |

## Contoh

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### Lihat Juga

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../aesecryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`AesEcryptionSettings`](../) tanpa kata sandi.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| metode | EncryptionMethod | Opsi algoritma yang menunjukkan ukuran blok cipher. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| NotSupportedException | *method* bukan salah satu dari AES128, AES192, atau AES256. |

### Lihat Juga

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../aesecryptionsettings/)
* assembly [Aspose.Zip](../../../)


