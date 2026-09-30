---
title: "XarFileEntry.CompressionProgressed"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "XarFileEntry olayı. Ham akışın bir kısmı sıkıştırıldığında tetiklenir"
type: docs
weight: 20
url: /tr/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

Ham akışın bir bölümü sıkıştırıldığında ortaya çıkar.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Açıklamalar

Olay göndericisi bir [`XarFileEntry`](../) örneğidir.

## Örnekler

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Ayrıca Bakınız

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


