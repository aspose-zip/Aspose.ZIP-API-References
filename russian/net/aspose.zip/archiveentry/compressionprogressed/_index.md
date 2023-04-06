---
title: ArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP для справочника API .NET
description: ArchiveEntry событие. Возникает при сжатии части необработанного потока.
type: docs
weight: 80
url: /ru/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Возникает при сжатии части необработанного потока.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Примечания

Отправителем события является[`ArchiveEntry`](../) пример.

### Примеры

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Смотрите также

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* пространство имен [Aspose.Zip](../../archiveentry/)
* сборка [Aspose.Zip](../../../)


