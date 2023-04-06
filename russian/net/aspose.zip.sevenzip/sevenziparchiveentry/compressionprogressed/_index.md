---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP для справочника API .NET
description: SevenZipArchiveEntry событие. Возникает при сжатии части необработанного потока.
type: docs
weight: 70
url: /ru/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Возникает при сжатии части необработанного потока.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Примечания

Отправителем события является[`SevenZipArchiveEntry`](../) пример.

### Примеры

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Смотрите также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* пространство имен [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* сборка [Aspose.Zip](../../../)


