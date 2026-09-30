---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "ZArchiveLoadOptions olayı. Bazı baytlar çıkarıldığında çağrılan temsilciyi alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

Bazı baytlar çıkarıldığında çağrılan temsilciyi alır veya ayarlar.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Açıklamalar

Olay göndericisi, çıkarma işlemi ilerleyen [`ZArchive`](../../zarchive/) örneğidir.

## Örnekler

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Ayrıca Bakınız

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


