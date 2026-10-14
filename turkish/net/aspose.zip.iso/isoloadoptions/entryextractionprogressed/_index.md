---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "IsoLoadOptions özelliği. Bazı baytlar çıkarıldığında çağrılan temsilciyi alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

Bazı baytlar çıkarıldığında çağrılan temsilciyi alır veya ayarlar.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Açıklamalar

Olay göndericisi, çıkarma ilerleyen [`IsoEntry`](../../isoentry/) örneğidir.

## Örnekler

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### Ayrıca Bakınız

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


