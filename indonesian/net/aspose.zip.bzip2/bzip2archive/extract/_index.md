---
title: Bzip2Archive.Extract
second_title: Aspose.ZIP untuk Referensi .NET API
description: Bzip2Archive metode. Mengekstrak arsip ke aliran yang disediakan.
type: docs
weight: 30
url: /id/net/aspose.zip.bzip2/bzip2archive/extract/
---
## Bzip2Archive.Extract method

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
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### Lihat juga

* class [Bzip2Archive](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2archive/)
* perakitan [Aspose.Zip](../../../)


