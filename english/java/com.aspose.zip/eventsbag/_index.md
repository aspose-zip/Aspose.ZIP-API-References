---
title: EventsBag
second_title: Aspose.ZIP for Java API Reference
description: Events container used on  saving.
type: docs
weight: 30
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
| [getEntryCompressed()](#getEntryCompressed--) | Gets an event that is raised after an archive entry has been compressed. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | Gets an event that is raised after an archive entry has been compressed. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


Gets an event that is raised after an archive entry has been compressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed.
### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


Gets an event that is raised after an archive entry has been compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | an event that is raised after an archive entry has been compressed. |

