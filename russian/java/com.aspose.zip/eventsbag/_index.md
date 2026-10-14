---
title: "EventsBag"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Контейнер событий, используемый при сохранении."
type: docs
weight: 65
url: /ru/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

Контейнер событий, используемый при сохранении [Archive](../../com.aspose.zip/archive).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Получает событие, которое вызывается перед сжатием записи архива. |
| [getEntryCompressed()](#getEntryCompressed--) | Получает событие, которое вызывается после сжатия записи архива. |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Устанавливает событие, которое вызывается перед сжатием записи архива. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | Устанавливает событие, которое вызывается после сжатия записи архива. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


Получает событие, которое вызывается перед сжатием записи архива.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


Получает событие, которое вызывается после сжатия записи архива.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


Устанавливает событие, которое вызывается перед сжатием записи архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | событие, которое вызывается до сжатия записи архива. |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


Устанавливает событие, которое вызывается после сжатия записи архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | событие, которое вызывается после того, как запись архива была сжата |

