---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Событие LzmaArchiveSettings. Вызывается, когда часть необработанного потока сжата."
type: docs
weight: 50
url: /ru/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

Вызывается, когда часть необработанного потока сжата.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Примеры

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### См. также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


