---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Bzip2SaveOptions olayı. Ham akışın bir bölümü sıkıştırıldığında tetiklenir"
type: docs
weight: 40
url: /tr/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

Ham akışın bir bölümü sıkıştırıldığında ortaya çıkar.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Açıklamalar

Bu olay çok iş parçacıklı modda sıkıştırma yapıldığında tetiklenmez.

## Örnekler

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Ayrıca Bakınız

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


