---
title: ArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP untuk Referensi .NET API
description: ArchiveEntry peristiwa. Muncul saat sebagian aliran mentah dikompresi.
type: docs
weight: 80
url: /id/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Muncul saat sebagian aliran mentah dikompresi.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Perkataan

Pengirim acara adalah[`ArchiveEntry`](../) contoh.

### Contoh

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Lihat juga

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* ruang nama [Aspose.Zip](../../archiveentry/)
* perakitan [Aspose.Zip](../../../)


