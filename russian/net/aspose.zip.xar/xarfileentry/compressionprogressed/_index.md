---
title: "XarFileEntry.CompressionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Событие XarFileEntry. Возникает, когда часть необработанного потока сжата"
type: docs
weight: 20
url: /ru/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

Вызывается, когда часть необработанного потока сжата.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Примечания

Отправитель события — экземпляр [`XarFileEntry`](../).

## Примеры

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### См. также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


