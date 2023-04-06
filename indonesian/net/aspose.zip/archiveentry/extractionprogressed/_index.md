---
title: ArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP untuk Referensi .NET API
description: ArchiveEntry peristiwa. Muncul saat sebagian aliran mentah diekstrak.
type: docs
weight: 90
url: /id/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Muncul saat sebagian aliran mentah diekstrak.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Perkataan

Pengirim acara adalah[`ArchiveEntry`](../) contoh.

### Contoh

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### Lihat juga

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* ruang nama [Aspose.Zip](../../archiveentry/)
* perakitan [Aspose.Zip](../../../)


