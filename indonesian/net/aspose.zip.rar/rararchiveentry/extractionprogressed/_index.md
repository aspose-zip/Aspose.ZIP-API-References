---
title: RarArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP untuk Referensi .NET API
description: RarArchiveEntry peristiwa. Muncul saat sebagian aliran mentah diekstrak.
type: docs
weight: 80
url: /id/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Muncul saat sebagian aliran mentah diekstrak.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Perkataan

Pengirim acara adalah[`RarArchiveEntry`](../) contoh.

### Contoh

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### Lihat juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* ruang nama [Aspose.Zip.Rar](../../rararchiveentry/)
* perakitan [Aspose.Zip](../../../)


