---
title: ArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP for .NET API Referansı
description: ArchiveEntry etkinlik. Ham akışın bir kısmı çıkarıldığında yükselir.
type: docs
weight: 90
url: /tr/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Ham akışın bir kısmı çıkarıldığında yükselir.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Notlar

Olay gönderen bir[`ArchiveEntry`](../) misal.

### Örnekler

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### Ayrıca bakınız

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* ad alanı [Aspose.Zip](../../archiveentry/)
* toplantı [Aspose.Zip](../../../)


