---
title: "ArchiveLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство ArchiveLoadOptions. Возвращает или задает делегат, вызываемый при извлечении некоторого количества байтов"
type: docs
weight: 50
url: /ru/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Получает или задает делегат, вызываемый после извлечения некоторых байтов.

```csharp
public EventHandler<ProgressCancelEventArgs> EntryExtractionProgressed { get; set; }
```

## Примечания

Отправитель события — экземпляр [`ArchiveEntry`](../../archiveentry/), для которого процесс извлечения продвигается.

## Примеры

Отслеживайте прогресс извлечения записи.

```csharp
var archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

Отмените извлечение записи после определённого времени.

```csharp
Stopwatch watch = Stopwatch.StartNew();
using (Archive a = new Archive("big.zip", new ArchiveLoadOptions() {
    EntryExtractionProgressed = (s, e) => { if (watch.ElapsedMilliseconds > 1000) e.Cancel = true; } }))
{
    a.Entries[0].Extract("first.bin");
}
```

### См. также

* class [ProgressCancelEventArgs](../../progresscanceleventargs/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


