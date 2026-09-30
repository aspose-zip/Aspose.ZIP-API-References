---
title: "ZstandardSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "ZstandardSaveOptions olayı. Ham akışın bir bölümü sıkıştırıldığında tetiklenir"
type: docs
weight: 20
url: /tr/net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

Ham akışın bir bölümü sıkıştırıldığında ortaya çıkar.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Örnekler

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Ayrıca Bakınız

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


