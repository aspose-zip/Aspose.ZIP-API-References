---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "XarLoadOptions özelliği. Bazı baytlar çıkarıldığında çağrılan temsilciyi alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

Bazı baytlar çıkarıldığında çağrılan temsilciyi alır veya ayarlar.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Açıklamalar

Olay göndericisi, çıkarma ilerleyen [`XarFileEntry`](../../xarfileentry/) örneğidir.

## Örnekler

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### Ayrıca Bakınız

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


