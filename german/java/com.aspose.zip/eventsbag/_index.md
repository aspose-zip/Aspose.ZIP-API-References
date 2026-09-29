---
title: "EventsBag"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Ereigniscontainer, der beim Speichern verwendet wird."
type: docs
weight: 65
url: /de/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

Ereigniscontainer, der beim Speichern von [Archive](../../com.aspose.zip/archive) verwendet wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Ruft ein Ereignis ab, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird. |
| [getEntryCompressed()](#getEntryCompressed--) | Ruft ein Ereignis ab, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde. |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


Ruft ein Ereignis ab, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


Ruft ein Ereignis ab, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


Setzt ein Ereignis, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | ein Ereignis, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird. |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


Setzt ein Ereignis, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | ein Ereignis, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde |

