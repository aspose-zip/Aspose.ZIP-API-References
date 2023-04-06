---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: TraditionalEncryptionSettings konstruktor. Menginisialisasi instance baru dariTraditionalEncryptionSettings kelas.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Menginisialisasi instance baru dari[`TraditionalEncryptionSettings`](../) kelas.

```csharp
public TraditionalEncryptionSettings(string password)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| password | String | Kata sandi untuk enkripsi. |

### Contoh

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Lihat juga

* class [TraditionalEncryptionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* perakitan [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Menginisialisasi instance baru dari[`TraditionalEncryptionSettings`](../) kelas dengan pengkodean yang ditentukan pengguna.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| password | String | Kata sandi untuk enkripsi. |
| encoding | Encoding | Pengkodean untuk karakter kata sandi. |

### Perkataan

Penggunaan konstruktor ini tidak disarankan. Mengatur pengkodean dapat bertentangan dengan standar dan menghasilkan arsip yang tidak kompatibel.

### Contoh

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Lihat juga

* class [TraditionalEncryptionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* perakitan [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Menginisialisasi instance baru dari[`TraditionalEncryptionSettings`](../)kelas tanpa password.

```csharp
public TraditionalEncryptionSettings()
```

### Lihat juga

* class [TraditionalEncryptionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* perakitan [Aspose.Zip](../../../)


