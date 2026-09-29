---
title: "EventsBagIso"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Ereigniscontainer, der beim Speichern verwendet wird."
type: docs
weight: 66
url: /de/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

Ereignisbehälter, der beim Speichern von [IsoArchive](../../com.aspose.zip/isoarchive) verwendet wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Ruft ein Ereignis ab, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird. |
| [getEntryCompressed()](#getEntryCompressed--) | Ruft ein Ereignis ab, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Setzt ein Ereignis, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Setzt ein Ereignis, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


Ruft ein Ereignis ab, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


Ruft ein Ereignis ab, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


Setzt ein Ereignis, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | ein Ereignis, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


Setzt ein Ereignis, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | ein Ereignis, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde |

