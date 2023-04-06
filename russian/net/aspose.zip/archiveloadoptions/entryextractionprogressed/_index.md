---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP для справочника API .NET
description: ArchiveLoadOptions свойство. Получает или задает делегат вызываемый после извлечения нескольких байтов.
type: docs
weight: 40
url: /ru/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Получает или задает делегат, вызываемый после извлечения нескольких байтов.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### Примечания

Отправителем события является[`ArchiveEntry`](../../archiveentry/) экземпляр, в котором выполняется извлечение.

### Примеры

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### Смотрите также

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* пространство имен [Aspose.Zip](../../archiveloadoptions/)
* сборка [Aspose.Zip](../../../)


