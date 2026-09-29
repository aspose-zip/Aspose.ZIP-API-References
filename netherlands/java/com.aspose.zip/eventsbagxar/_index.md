---
title: "EventsBagXar"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Evenementencontainer gebruikt bij het opslaan."
type: docs
weight: 67
url: /nl/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

Evenementencontainer gebruikt bij het opslaan van [XarArchive](../../com.aspose.zip/xararchive).
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Haalt een gebeurtenis op die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd. |
| [getEntryCompressed()](#getEntryCompressed--) | Haalt een gebeurtenis op die wordt geactiveerd nadat een archiefitem is gecomprimeerd. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | Stelt een gebeurtenis in die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | Stelt een gebeurtenis in die wordt geactiveerd nadat een archiefitem is gecomprimeerd. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


Haalt een gebeurtenis op die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


Haalt een gebeurtenis op die wordt geactiveerd nadat een archiefitem is gecomprimeerd.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


Stelt een gebeurtenis in die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | een gebeurtenis die wordt geactiveerd voordat een archiefitem wordt gecomprimeerd. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


Stelt een gebeurtenis in die wordt geactiveerd nadat een archiefitem is gecomprimeerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | een gebeurtenis die wordt geactiveerd nadat een archiefitem is gecomprimeerd |

