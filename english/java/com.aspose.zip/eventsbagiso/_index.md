---
title: EventsBagIso
second_title: Aspose.ZIP for Java API Reference
description: Events container used on  saving.
type: docs
weight: 44
url: /java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

Events container used on [IsoArchive](../../com.aspose.zip/isoarchive) saving.
## Constructors

| Constructor | Description |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Gets an event that is raised before an archive entry is being compressed. |
| [getEntryCompressed()](#getEntryCompressed--) | Gets an event that is raised after an archive entry has been compressed. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Sets an event that is raised before an archive entry is being compressed. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Sets an event that is raised after an archive entry has been compressed. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


Gets an event that is raised before an archive entry is being compressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


Gets an event that is raised after an archive entry has been compressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


Sets an event that is raised before an archive entry is being compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | an event that is raised before an archive entry is being compressed. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


Sets an event that is raised after an archive entry has been compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | an event that is raised after an archive entry has been compressed |

