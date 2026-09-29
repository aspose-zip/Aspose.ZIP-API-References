---
title: "EventsBagXar"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Контейнер событий, используемый при сохранении."
type: docs
weight: 67
url: /ru/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

Контейнер событий, используемый при сохранении [XarArchive](../../com.aspose.zip/xararchive).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Получает событие, которое вызывается перед сжатием записи архива. |
| [getEntryCompressed()](#getEntryCompressed--) | Получает событие, которое вызывается после сжатия записи архива. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | Устанавливает событие, которое вызывается перед сжатием записи архива. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | Устанавливает событие, которое вызывается после сжатия записи архива. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


Получает событие, которое вызывается перед сжатием записи архива.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


Получает событие, которое вызывается после сжатия записи архива.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


Устанавливает событие, которое вызывается перед сжатием записи архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | событие, которое вызывается до сжатия записи архива. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


Устанавливает событие, которое вызывается после сжатия записи архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | событие, которое вызывается после того, как запись архива была сжата |

