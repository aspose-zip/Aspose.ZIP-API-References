---
title: "TraditionalEncryptionSettings.TraditionalEncryptionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor TraditionalEncryptionSettings. Menginisialisasi instance baru dari kelas TraditionalEncryptionSettings"
type: docs
weight: 10
url: /id/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Menginisialisasi instance baru dari kelas [`TraditionalEncryptionSettings`](../).

```csharp
public TraditionalEncryptionSettings(string password)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| password | String | Kata sandi untuk enkripsi. |

## Contoh

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Lihat Juga

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Menginisialisasi instance baru dari kelas [`TraditionalEncryptionSettings`](../) dengan encoding yang ditentukan pengguna.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| password | String | Kata sandi untuk enkripsi. |
| encoding | Pengkodean | Pengkodean untuk karakter kata sandi. |

## Catatan

Penggunaan konstruktor ini tidak disarankan. Menetapkan pengkodean dapat bertentangan dengan standar dan menghasilkan arsip yang tidak kompatibel.

## Contoh

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Lihat Juga

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Menginisialisasi instance baru dari kelas [`TraditionalEncryptionSettings`](../) tanpa kata sandi.

```csharp
public TraditionalEncryptionSettings()
```

### Lihat Juga

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)


