---
title: ArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP for .NET API Referansı
description: ArchiveEntry etkinlik. Ham akışın bir kısmı sıkıştırıldığında yükselir.
type: docs
weight: 80
url: /tr/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Ham akışın bir kısmı sıkıştırıldığında yükselir.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Notlar

Olay gönderen bir[`ArchiveEntry`](../) misal.

### Örnekler

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Ayrıca bakınız

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* ad alanı [Aspose.Zip](../../archiveentry/)
* toplantı [Aspose.Zip](../../../)


