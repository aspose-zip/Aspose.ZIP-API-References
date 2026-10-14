---
title: "CancelEntryEventArgs"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Аргументы события для отменяемых событий, связанных с записью."
type: docs
weight: 52
url: /ru/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

Аргументы события для отменяемых событий, связанных с записью.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | Инициализирует новый экземпляр класса [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## Методы

| Метод | Описание |
| --- | --- |
| [getCancel()](#getCancel--) | Возвращает значение, указывающее, следует ли отменить событие. |
| [setCancel(boolean value)](#setCancel-boolean-) | Устанавливает значение, указывающее, следует ли отменить событие. |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


Инициализирует новый экземпляр класса [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Элемент архива, для которого вызывается событие. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Возвращает значение, указывающее, следует ли отменить событие.

**Returns:**
boolean — true, если событие следует отменить; иначе false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Устанавливает значение, указывающее, следует ли отменить событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | true, если событие следует отменить; иначе false. |

