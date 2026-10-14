---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "XarBzip2CompressionSettings constructor. Menginisialisasi sebuah instance baru dari kelas XarBzip2CompressionSettings"
type: docs
weight: 10
url: /id/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`XarBzip2CompressionSettings`](../).

```csharp
public XarBzip2CompressionSettings(int blockSize)
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
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### Lihat Juga

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`XarBzip2CompressionSettings`](../) dengan ukuran blok default, yaitu 9 ratus kilobita.

```csharp
public XarBzip2CompressionSettings()
```

### Lihat Juga

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


