---
title: GzipArchive.Extract
second_title: Aspose.ZIP untuk Referensi .NET API
description: GzipArchive metode. Mengekstrak arsip ke aliran yang disediakan.
type: docs
weight: 40
url: /id/net/aspose.zip.gzip/gziparchive/extract/
---
## GzipArchive.Extract method

Mengekstrak arsip ke aliran yang disediakan.

```csharp
public void Extract(Stream destination)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destination | Stream | Aliran tujuan. Harus dapat ditulis. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *destination* tidak mendukung penulisan. |

### Contoh

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### Lihat juga

* class [GzipArchive](../)
* ruang nama [Aspose.Zip.Gzip](../../gziparchive/)
* perakitan [Aspose.Zip](../../../)


