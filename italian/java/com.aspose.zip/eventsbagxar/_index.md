---
title: "EventsBagXar"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Contenitore di eventi utilizzato durante il salvataggio."
type: docs
weight: 67
url: /it/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

Contenitore di eventi utilizzato durante il salvataggio di [XarArchive](../../com.aspose.zip/xararchive).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Ottiene un evento che viene sollevato prima che una voce di archivio venga compressa. |
| [getEntryCompressed()](#getEntryCompressed--) | Ottiene un evento che viene sollevato dopo che una voce di archivio è stata compressa. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | Imposta un evento che viene sollevato prima che una voce di archivio venga compressa. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | Imposta un evento che viene sollevato dopo che una voce di archivio è stata compressa. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


Ottiene un evento che viene sollevato prima che una voce di archivio venga compressa.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


Ottiene un evento che viene sollevato dopo che una voce di archivio è stata compressa.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


Imposta un evento che viene sollevato prima che una voce di archivio venga compressa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | un evento che viene sollevato prima che una voce dell'archivio venga compressa. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


Imposta un evento che viene sollevato dopo che una voce di archivio è stata compressa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | un evento che viene sollevato dopo che una voce dell'archivio è stata compressa |

