---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "LzmaArchiveSettings olayı. Ham akışın bir kısmı sıkıştırıldığında tetiklenir"
type: docs
weight: 50
url: /tr/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

Ham akışın bir bölümü sıkıştırıldığında ortaya çıkar.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Örnekler

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Ayrıca Bakınız

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


