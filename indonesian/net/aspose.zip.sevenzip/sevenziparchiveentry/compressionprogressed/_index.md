---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP untuk Referensi .NET API
description: SevenZipArchiveEntry peristiwa. Muncul saat sebagian aliran mentah dikompresi.
type: docs
weight: 70
url: /id/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Muncul saat sebagian aliran mentah dikompresi.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Perkataan

Pengirim acara adalah[`SevenZipArchiveEntry`](../) contoh.

### Contoh

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Lihat juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* perakitan [Aspose.Zip](../../../)


