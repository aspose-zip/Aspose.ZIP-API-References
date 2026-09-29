---
title: "EventsBag"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Conteneur d'événements utilisé lors de l'enregistrement."
type: docs
weight: 65
url: /fr/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

Conteneur d'événements utilisé lors de l'enregistrement de [Archive](../../com.aspose.zip/archive).
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Obtient un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée. |
| [getEntryCompressed()](#getEntryCompressed--) | Obtient un événement qui est déclenché après qu'une entrée d'archive a été compressée. |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Définit un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | Définit un événement qui est déclenché après qu'une entrée d'archive a été compressée. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


Obtient un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


Obtient un événement qui est déclenché après qu'une entrée d'archive a été compressée.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


Définit un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée. |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


Définit un événement qui est déclenché après qu'une entrée d'archive a été compressée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | un événement qui est déclenché après qu'une entrée d'archive a été compressée |

