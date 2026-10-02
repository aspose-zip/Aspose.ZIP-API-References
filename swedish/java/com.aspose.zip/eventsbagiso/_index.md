---
title: "EventsBagIso"
second_title: "Aspose.ZIP för Java API-referens"
description: "Evenemangsbehållare som används vid sparning."
type: docs
weight: 66
url: /sv/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

Evenemangsbehållare som används vid sparande av [IsoArchive](../../com.aspose.zip/isoarchive).
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Hämtar ett evenemang som utlöses innan ett arkivinlägg komprimeras. |
| [getEntryCompressed()](#getEntryCompressed--) | Hämtar ett evenemang som utlöses efter att ett arkivinlägg har komprimerats. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Ställer in ett evenemang som utlöses innan ett arkivinlägg komprimeras. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Ställer in ett evenemang som utlöses efter att ett arkivinlägg har komprimerats. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


Hämtar ett evenemang som utlöses innan ett arkivinlägg komprimeras.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


Hämtar ett evenemang som utlöses efter att ett arkivinlägg har komprimerats.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


Ställer in ett evenemang som utlöses innan ett arkivinlägg komprimeras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | en händelse som utlöses innan ett arkivinlägg komprimeras. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


Ställer in ett evenemang som utlöses efter att ett arkivinlägg har komprimerats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | en händelse som utlöses efter att ett arkivinlägg har komprimerats |

