---
title: "EventsBagXar"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Conteneur d'événements utilisé lors de l'enregistrement."
type: docs
weight: 67
url: /fr/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

Conteneur d'événements utilisé lors de l'enregistrement de [XarArchive](../../com.aspose.zip/xararchive).
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Obtient un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée. |
| [getEntryCompressed()](#getEntryCompressed--) | Obtient un événement qui est déclenché après qu'une entrée d'archive a été compressée. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | Définit un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | Définit un événement qui est déclenché après qu'une entrée d'archive a été compressée. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


Obtient un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


Obtient un événement qui est déclenché après qu'une entrée d'archive a été compressée.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


Définit un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | un événement qui est déclenché avant qu'une entrée d'archive ne soit compressée. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


Définit un événement qui est déclenché après qu'une entrée d'archive a été compressée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | un événement qui est déclenché après qu'une entrée d'archive a été compressée |

