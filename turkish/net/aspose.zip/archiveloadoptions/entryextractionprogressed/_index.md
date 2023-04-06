---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP for .NET API Referansı
description: ArchiveLoadOptions mülk. Bazı baytlar ayıklandığında çağrılan temsilciyi alır veya ayarlar.
type: docs
weight: 40
url: /tr/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Bazı baytlar ayıklandığında çağrılan temsilciyi alır veya ayarlar.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### Notlar

Olay göndereni[`ArchiveEntry`](../../archiveentry/) çıkarmanın ilerlediği örnek.

### Örnekler

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### Ayrıca bakınız

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* ad alanı [Aspose.Zip](../../archiveloadoptions/)
* toplantı [Aspose.Zip](../../../)


