---
title: EventsBag
second_title: Aspose.ZIP for Java API Reference
description: Events container used on  saving.
type: docs
weight: 40
url: /java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

Events container used on [Archive](../../com.aspose.zip/archive) saving.
## Constructors

| Constructor | Description |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Gets an event that is raised before an archive entry is being compressed. |
| [getEntryCompressed()](#getEntryCompressed--) | Gets an event that is raised after an archive entry has been compressed. |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Sets an event that is raised before an archive entry is being compressed. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | Sets an event that is raised after an archive entry has been compressed. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


Gets an event that is raised before an archive entry is being compressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


Gets an event that is raised after an archive entry has been compressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


Sets an event that is raised before an archive entry is being compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | an event that is raised before an archive entry is being compressed. |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


Sets an event that is raised after an archive entry has been compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | an event that is raised after an archive entry has been compressed |

