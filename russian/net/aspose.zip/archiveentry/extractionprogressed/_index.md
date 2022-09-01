---
title: ExtractionProgressed
second_title: Aspose.ZIP для справочника API .NET
description: Возникает при извлечении части исходного потока.
type: docs
weight: 80
url: /ru/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Возникает при извлечении части исходного потока.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Примечания

Отправителем события является экземпляр[`ArchiveEntry`](../../archiveentry).

### Примеры

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### Смотрите также

* class [ProgressEventArgs](../../progresseventargs)
* class [ArchiveEntry](../../archiveentry)
* пространство имен [Aspose.Zip](../../archiveentry)
* сборка [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->