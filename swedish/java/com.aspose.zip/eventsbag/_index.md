---
title: "EventsBag"
second_title: "Aspose.ZIP för Java API-referens"
description: "Evenemangsbehållare som används vid sparning."
type: docs
weight: 65
url: /sv/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

Evenemangskontainer som används vid sparande av [Archive](../../com.aspose.zip/archive).
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Hämtar ett evenemang som utlöses innan ett arkivinlägg komprimeras. |
| [getEntryCompressed()](#getEntryCompressed--) | Hämtar ett evenemang som utlöses efter att ett arkivinlägg har komprimerats. |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Ställer in ett evenemang som utlöses innan ett arkivinlägg komprimeras. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | Ställer in ett evenemang som utlöses efter att ett arkivinlägg har komprimerats. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


Hämtar ett evenemang som utlöses innan ett arkivinlägg komprimeras.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


Hämtar ett evenemang som utlöses efter att ett arkivinlägg har komprimerats.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


Ställer in ett evenemang som utlöses innan ett arkivinlägg komprimeras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | en händelse som utlöses innan ett arkivinlägg komprimeras. |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


Ställer in ett evenemang som utlöses efter att ett arkivinlägg har komprimerats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | en händelse som utlöses efter att ett arkivinlägg har komprimerats |

