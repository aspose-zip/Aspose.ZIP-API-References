---
title: "EventsBag"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Evenementencontainer gebruikt bij het opslaan."
type: docs
weight: 65
url: /nl/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

Evenementencontainer gebruikt bij het opslaan van [Archive](../../com.aspose.zip/archive).
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Haalt een gebeurtenis op die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd. |
| [getEntryCompressed()](#getEntryCompressed--) | Haalt een gebeurtenis op die wordt geactiveerd nadat een archiefitem is gecomprimeerd. |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Stelt een gebeurtenis in die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | Stelt een gebeurtenis in die wordt geactiveerd nadat een archiefitem is gecomprimeerd. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


Haalt een gebeurtenis op die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


Haalt een gebeurtenis op die wordt geactiveerd nadat een archiefitem is gecomprimeerd.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


Stelt een gebeurtenis in die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | een gebeurtenis die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd. |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


Stelt een gebeurtenis in die wordt geactiveerd nadat een archiefitem is gecomprimeerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | een gebeurtenis die wordt geactiveerd nadat een archiefitem is gecomprimeerd |

