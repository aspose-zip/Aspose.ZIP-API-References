---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Событие Bzip2SaveOptions. Вызывается, когда часть необработанного потока сжата."
type: docs
weight: 40
url: /ru/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

Вызывается, когда часть необработанного потока сжата.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Примечания

Это событие не будет вызываться при сжатии в многопоточном режиме.

## Примеры

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### См. также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


