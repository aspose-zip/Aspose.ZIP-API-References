---
title: "EventsBagIso"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Contenitore di eventi utilizzato durante il salvataggio."
type: docs
weight: 66
url: /it/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

Contenitore di eventi utilizzato durante il salvataggio di [IsoArchive](../../com.aspose.zip/isoarchive).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Ottiene un evento che viene sollevato prima che una voce di archivio venga compressa. |
| [getEntryCompressed()](#getEntryCompressed--) | Ottiene un evento che viene sollevato dopo che una voce di archivio è stata compressa. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Imposta un evento che viene sollevato prima che una voce di archivio venga compressa. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Imposta un evento che viene sollevato dopo che una voce di archivio è stata compressa. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


Ottiene un evento che viene sollevato prima che una voce di archivio venga compressa.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


Ottiene un evento che viene sollevato dopo che una voce di archivio è stata compressa.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


Imposta un evento che viene sollevato prima che una voce di archivio venga compressa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | un evento che viene sollevato prima che una voce dell'archivio venga compressa. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


Imposta un evento che viene sollevato dopo che una voce di archivio è stata compressa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | un evento che viene sollevato dopo che una voce dell'archivio è stata compressa |

