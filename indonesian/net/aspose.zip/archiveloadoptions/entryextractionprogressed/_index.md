---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP untuk Referensi .NET API
description: ArchiveLoadOptions Properti. Mendapatkan atau menyetel delegasi yang dipanggil saat beberapa byte telah diekstrak.
type: docs
weight: 40
url: /id/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Mendapatkan atau menyetel delegasi yang dipanggil saat beberapa byte telah diekstrak.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### Perkataan

Pengirim acara adalah[`ArchiveEntry`](../../archiveentry/) contoh yang ekstraksi maju.

### Contoh

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### Lihat juga

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* ruang nama [Aspose.Zip](../../archiveloadoptions/)
* perakitan [Aspose.Zip](../../../)


