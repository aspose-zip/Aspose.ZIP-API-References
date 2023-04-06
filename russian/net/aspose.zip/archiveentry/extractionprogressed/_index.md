---
title: ArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP для справочника API .NET
description: ArchiveEntry событие. Возникает при извлечении части необработанного потока.
type: docs
weight: 90
url: /ru/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Возникает при извлечении части необработанного потока.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Примечания

Отправителем события является[`ArchiveEntry`](../) пример.

### Примеры

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### Смотрите также

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* пространство имен [Aspose.Zip](../../archiveentry/)
* сборка [Aspose.Zip](../../../)


