---
title: "EventsBagXar"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Ereigniscontainer, der beim Speichern verwendet wird."
type: docs
weight: 67
url: /de/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

Ereigniscontainer, der beim Speichern von [XarArchive](../../com.aspose.zip/xararchive) verwendet wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Ruft ein Ereignis ab, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird. |
| [getEntryCompressed()](#getEntryCompressed--) | Ruft ein Ereignis ab, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | Setzt ein Ereignis, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | Setzt ein Ereignis, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


Ruft ein Ereignis ab, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


Ruft ein Ereignis ab, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


Setzt ein Ereignis, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | ein Ereignis, das ausgelöst wird, bevor ein Archiveintrag komprimiert wird. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


Setzt ein Ereignis, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | ein Ereignis, das ausgelöst wird, nachdem ein Archiveintrag komprimiert wurde |

