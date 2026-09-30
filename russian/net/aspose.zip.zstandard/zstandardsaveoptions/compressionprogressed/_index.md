---
title: "ZstandardSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Событие ZstandardSaveOptions. Вызывается, когда часть необработанного потока сжата"
type: docs
weight: 20
url: /ru/net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

Вызывается, когда часть необработанного потока сжата.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Примеры

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### См. также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


