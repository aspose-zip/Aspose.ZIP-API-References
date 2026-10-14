---
title: "EventsBagIso"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Evenementencontainer gebruikt bij het opslaan."
type: docs
weight: 66
url: /nl/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

Evenementencontainer gebruikt bij het opslaan van [IsoArchive](../../com.aspose.zip/isoarchive).
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Haalt een gebeurtenis op die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd. |
| [getEntryCompressed()](#getEntryCompressed--) | Haalt een gebeurtenis op die wordt geactiveerd nadat een archiefitem is gecomprimeerd. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Stelt een gebeurtenis in die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Stelt een gebeurtenis in die wordt geactiveerd nadat een archiefitem is gecomprimeerd. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


Haalt een gebeurtenis op die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


Haalt een gebeurtenis op die wordt geactiveerd nadat een archiefitem is gecomprimeerd.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


Stelt een gebeurtenis in die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | een gebeurtenis die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


Stelt een gebeurtenis in die wordt geactiveerd nadat een archiefitem is gecomprimeerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | een gebeurtenis die wordt geactiveerd nadat een archiefitem is gecomprimeerd |

