---
title: "ArchiveLoadOptions.EntryListed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство ArchiveLoadOptions. Возвращает или задает делегат, вызываемый, когда запись перечислена в таблице содержимого."
type: docs
weight: 60
url: /ru/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

Получает или задает делегат, вызываемый при перечислении записи в таблице содержимого.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

## Примеры

```csharp
var archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### См. также

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


