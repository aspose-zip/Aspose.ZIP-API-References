---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "ZstandardLoadOptions olayı. Bazı baytlar çıkarıldığında çağrılan temsilciyi alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

Bazı baytlar çıkarıldığında çağrılan temsilciyi alır veya ayarlar.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Açıklamalar

Olay göndericisi, çıkarımı ilerleyen [`ZstandardArchive`](../../zstandardarchive/) örneğidir.

## Örnekler

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Ayrıca Bakınız

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


