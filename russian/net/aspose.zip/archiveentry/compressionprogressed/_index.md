---
title: "ArchiveEntry.CompressionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Событие ArchiveEntry. Возникает, когда часть необработанного потока сжата"
type: docs
weight: 90
url: /ru/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Вызывается, когда часть необработанного потока сжата.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Примечания

Отправитель события — экземпляр [`ArchiveEntry`](../).

## Примеры

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### См. также

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


