---
title: "ProgressCancelEventArgs"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Класс для отменяемых данных события, содержащих количество обработанных байт."
type: docs
weight: 95
url: /ru/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

Класс для отменяемых данных события, содержащих количество обработанных байт.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | Инициализирует новый экземпляр класса [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs). |
## Методы

| Метод | Описание |
| --- | --- |
| [getCancel()](#getCancel--) | Возвращает значение, указывающее, следует ли отменить событие. |
| [setCancel(boolean value)](#setCancel-boolean-) | Устанавливает значение, указывающее, следует ли отменить событие. |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


Инициализирует новый экземпляр класса [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| proceededBytes | long | Количество обработанных байтов. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Возвращает значение, указывающее, следует ли отменить событие.

**Returns:**
boolean — True, если событие должно быть отменено; иначе false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Устанавливает значение, указывающее, следует ли отменить событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | значение, указывающее, должно ли событие быть отменено. |

