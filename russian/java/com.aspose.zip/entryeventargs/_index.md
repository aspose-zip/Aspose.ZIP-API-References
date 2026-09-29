---
title: "EntryEventArgs"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Аргументы события для событий, связанных с записью."
type: docs
weight: 62
url: /ru/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

Аргументы события для событий, связанных с записью.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | Инициализирует новый экземпляр класса [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Методы

| Метод | Описание |
| --- | --- |
| [getEntry()](#getEntry--) | Получает запись архива, для которой вызывается событие. |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


Инициализирует новый экземпляр класса [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Элемент архива, для которого вызывается событие. |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


Получает запись архива, для которой вызывается событие.

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
