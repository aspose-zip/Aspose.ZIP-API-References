---
title: "EventsBagIso"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Контейнер событий, используемый при сохранении."
type: docs
weight: 66
url: /ru/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

Контейнер событий, используемый при сохранении [IsoArchive](../../com.aspose.zip/isoarchive).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Получает событие, которое вызывается перед сжатием записи архива. |
| [getEntryCompressed()](#getEntryCompressed--) | Получает событие, которое вызывается после сжатия записи архива. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Устанавливает событие, которое вызывается перед сжатием записи архива. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Устанавливает событие, которое вызывается после сжатия записи архива. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


Получает событие, которое вызывается перед сжатием записи архива.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


Получает событие, которое вызывается после сжатия записи архива.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


Устанавливает событие, которое вызывается перед сжатием записи архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | событие, которое вызывается до сжатия записи архива. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


Устанавливает событие, которое вызывается после сжатия записи архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | событие, которое вызывается после того, как запись архива была сжата |

