---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: Bzip2CompressionSettings konstruktor. Menginisialisasi instance baru dariBzip2CompressionSettings kelas.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

Menginisialisasi instance baru dari[`Bzip2CompressionSettings`](../) kelas.

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| blockSize | Int32 | Ukuran blok dalam ratusan kilobyte. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | Ukuran blok tidak antara 1 dan 9. |

### Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Lihat juga

* class [Bzip2CompressionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* perakitan [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

Menginisialisasi instance baru dari[`Bzip2CompressionSettings`](../) kelas dengan ukuran blok default, sama dengan 9 ratus kilobyte.

```csharp
public Bzip2CompressionSettings()
```

### Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Lihat juga

* class [Bzip2CompressionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* perakitan [Aspose.Zip](../../../)


