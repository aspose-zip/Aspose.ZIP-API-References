---
title: "ZArchiveSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "ZArchiveSaveOptions olayı. Ham akışın bir bölümü sıkıştırıldığında tetiklenir"
type: docs
weight: 20
url: /tr/net/aspose.zip.z/zarchivesaveoptions/compressionprogressed/
---
## ZArchiveSaveOptions.CompressionProgressed event

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
* class [ZArchiveSaveOptions](../)
* namespace [Aspose.Zip.Z](../../zarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


