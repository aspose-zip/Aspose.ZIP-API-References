---
title: "CancelEntryEventArgsXar"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Аргументы события для отменяемых событий, связанных с записью."
type: docs
weight: 53
url: /ru/java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

Аргументы события для отменяемых событий, связанных с записью.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | Инициализирует новый экземпляр класса [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## Методы

| Метод | Описание |
| --- | --- |
| [getCancel()](#getCancel--) | Возвращает значение, указывающее, следует ли отменить событие. |
| [setCancel(boolean value)](#setCancel-boolean-) | Устанавливает значение, указывающее, следует ли отменить событие. |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


Инициализирует новый экземпляр класса [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | запись архива, для которой вызывается событие |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Возвращает значение, указывающее, следует ли отменить событие.

**Returns:**
boolean - true, если событие должно быть отменено; иначе false
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Устанавливает значение, указывающее, следует ли отменить событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | true, если событие должно быть отменено; иначе false |

