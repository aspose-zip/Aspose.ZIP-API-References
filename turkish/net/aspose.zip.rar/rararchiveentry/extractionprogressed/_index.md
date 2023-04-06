---
title: RarArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP for .NET API Referansı
description: RarArchiveEntry etkinlik. Ham akışın bir kısmı çıkarıldığında yükselir.
type: docs
weight: 80
url: /tr/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Ham akışın bir kısmı çıkarıldığında yükselir.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Notlar

Olay gönderen bir[`RarArchiveEntry`](../) misal.

### Örnekler

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### Ayrıca bakınız

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* ad alanı [Aspose.Zip.Rar](../../rararchiveentry/)
* toplantı [Aspose.Zip](../../../)


