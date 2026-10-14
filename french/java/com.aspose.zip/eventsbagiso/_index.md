---
title: "EventsBagIso"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Conteneur d'événements utilisé lors de l'enregistrement."
type: docs
weight: 66
url: /fr/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

Conteneur d'événements utilisé lors de l'enregistrement de [IsoArchive](../../com.aspose.zip/isoarchive).
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Obtient un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée. |
| [getEntryCompressed()](#getEntryCompressed--) | Obtient un événement qui est déclenché après qu'une entrée d'archive a été compressée. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Définit un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Définit un événement qui est déclenché après qu'une entrée d'archive a été compressée. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


Obtient un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


Obtient un événement qui est déclenché après qu'une entrée d'archive a été compressée.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


Définit un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


Définit un événement qui est déclenché après qu'une entrée d'archive a été compressée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | un événement qui est déclenché après qu'une entrée d'archive a été compressée |

