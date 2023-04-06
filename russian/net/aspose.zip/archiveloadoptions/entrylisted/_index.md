---
title: ArchiveLoadOptions.EntryListed
second_title: Aspose.ZIP для справочника API .NET
description: ArchiveLoadOptions свойство. Получает или задает делегата который вызывается когда запись указана в таблице содержания.
type: docs
weight: 50
url: /ru/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

Получает или задает делегата, который вызывается, когда запись указана в таблице содержания.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### Примеры

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### Смотрите также

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* пространство имен [Aspose.Zip](../../archiveloadoptions/)
* сборка [Aspose.Zip](../../../)


