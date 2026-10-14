---
title: "Bzip2CompressionSettings.Bzip2CompressionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor Bzip2CompressionSettings. Menginisialisasi instance baru dari kelas Bzip2CompressionSettings"
type: docs
weight: 10
url: /id/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

Menginisialisasi instance baru dari kelas [`Bzip2CompressionSettings`](../).

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| blockSize | Int32 | Ukuran blok dalam ratusan kilobyte. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | Ukuran blok tidak berada di antara 1 dan 9. |

## Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Lihat Juga

* class [Bzip2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

Menginisialisasi instance baru dari kelas [`Bzip2CompressionSettings`](../) dengan ukuran blok default, yaitu 9 ratus kilobyte.

```csharp
public Bzip2CompressionSettings()
```

## Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Lihat Juga

* class [Bzip2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


