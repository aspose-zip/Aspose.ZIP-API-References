---
title: "EventsBagXar"
second_title: "Aspose.ZIP för Java API-referens"
description: "Evenemangsbehållare som används vid sparning."
type: docs
weight: 67
url: /sv/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

Evenemangsbehållare som används vid sparning av [XarArchive](../../com.aspose.zip/xararchive).
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Hämtar ett evenemang som utlöses innan ett arkivinlägg komprimeras. |
| [getEntryCompressed()](#getEntryCompressed--) | Hämtar ett evenemang som utlöses efter att ett arkivinlägg har komprimerats. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | Ställer in ett evenemang som utlöses innan ett arkivinlägg komprimeras. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | Ställer in ett evenemang som utlöses efter att ett arkivinlägg har komprimerats. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


Hämtar ett evenemang som utlöses innan ett arkivinlägg komprimeras.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


Hämtar ett evenemang som utlöses efter att ett arkivinlägg har komprimerats.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


Ställer in ett evenemang som utlöses innan ett arkivinlägg komprimeras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | en händelse som utlöses innan ett arkivinlägg komprimeras. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


Ställer in ett evenemang som utlöses efter att ett arkivinlägg har komprimerats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | en händelse som utlöses efter att ett arkivinlägg har komprimerats |

