---
title: "EntryEventArgsIso"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Аргументы события для событий, связанных с записью."
type: docs
weight: 63
url: /ru/java/com.aspose.zip/entryeventargsiso/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsIso extends System.EventArgs
```

Аргументы события для событий, связанных с записью.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [EntryEventArgsIso(IsoEntry entry)](#EntryEventArgsIso-com.aspose.zip.IsoEntry-) | Инициализирует новый экземпляр класса [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Методы

| Метод | Описание |
| --- | --- |
| [getEntry()](#getEntry--) | Получает запись архива, для которой вызывается событие. |
### EntryEventArgsIso(IsoEntry entry) {#EntryEventArgsIso-com.aspose.zip.IsoEntry-}
```
public EntryEventArgsIso(IsoEntry entry)
```


Инициализирует новый экземпляр класса [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| entry | [IsoEntry](../../com.aspose.zip/isoentry) | запись архива, для которой вызывается событие |

### getEntry() {#getEntry--}
```
public final IsoEntry getEntry()
```


Получает запись архива, для которой вызывается событие.

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the archive entry the event is raised for
