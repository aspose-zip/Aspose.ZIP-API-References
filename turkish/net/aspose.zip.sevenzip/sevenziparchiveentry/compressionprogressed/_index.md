---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP for .NET API Referansı
description: SevenZipArchiveEntry etkinlik. Ham akışın bir kısmı sıkıştırıldığında yükselir.
type: docs
weight: 70
url: /tr/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Ham akışın bir kısmı sıkıştırıldığında yükselir.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Notlar

Olay gönderen bir[`SevenZipArchiveEntry`](../) misal.

### Örnekler

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Ayrıca bakınız

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* toplantı [Aspose.Zip](../../../)


