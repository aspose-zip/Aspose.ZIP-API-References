---
title: "EntryEventArgsXar"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Аргументы события для событий, связанных с записью."
type: docs
weight: 64
url: /ru/java/com.aspose.zip/entryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsXar extends System.EventArgs
```

Аргументы события для событий, связанных с записью.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [EntryEventArgsXar(XarEntry entry)](#EntryEventArgsXar-com.aspose.zip.XarEntry-) | Инициализирует новый экземпляр класса [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Методы

| Метод | Описание |
| --- | --- |
| [getEntry()](#getEntry--) | Получает запись архива, для которой вызывается событие. |
### EntryEventArgsXar(XarEntry entry) {#EntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public EntryEventArgsXar(XarEntry entry)
```


Инициализирует новый экземпляр класса [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | запись архива, для которой вызывается событие |

### getEntry() {#getEntry--}
```
public final XarEntry getEntry()
```


Получает запись архива, для которой вызывается событие.

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - the archive entry the event is raised for
