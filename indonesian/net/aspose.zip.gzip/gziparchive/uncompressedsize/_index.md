---
title: "GzipArchive.UncompressedSize"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti GzipArchive. Mendapatkan ukuran file asli"
type: docs
weight: 30
url: /id/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

Mendapatkan ukuran file asli.

```csharp
public ulong UncompressedSize { get; }
```

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

Selama dekompresi, properti ini mungkin berisi ukuran yang tidak tepat. Jika ukuran file yang tidak terkompresi melebihi 4GB, properti ini akan memberikan nilai yang salah karena batas 32-bit pada header.

### Lihat Juga

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


