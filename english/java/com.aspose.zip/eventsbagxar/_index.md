---
title: EventsBagXar
second_title: Aspose.ZIP for Java API Reference
description: Events container used on  saving.
type: docs
weight: 42
url: /java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

Events container used on [XarArchive](../../com.aspose.zip/xararchive) saving.
## Constructors

| Constructor | Description |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Gets an event that is raised before an archive entry is being compressed. |
| [getEntryCompressed()](#getEntryCompressed--) | Gets an event that is raised after an archive entry has been compressed. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | Sets an event that is raised before an archive entry is being compressed. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | Sets an event that is raised after an archive entry has been compressed. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


Gets an event that is raised before an archive entry is being compressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


Gets an event that is raised after an archive entry has been compressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


Sets an event that is raised before an archive entry is being compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | an event that is raised before an archive entry is being compressed. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


Sets an event that is raised after an archive entry has been compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | an event that is raised after an archive entry has been compressed |

