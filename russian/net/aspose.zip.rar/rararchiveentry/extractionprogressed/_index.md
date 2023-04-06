---
title: RarArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP для справочника API .NET
description: RarArchiveEntry событие. Возникает при извлечении части необработанного потока.
type: docs
weight: 80
url: /ru/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Возникает при извлечении части необработанного потока.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Примечания

Отправителем события является[`RarArchiveEntry`](../) пример.

### Примеры

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### Смотрите также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* пространство имен [Aspose.Zip.Rar](../../rararchiveentry/)
* сборка [Aspose.Zip](../../../)


