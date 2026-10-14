---
title: "EventsBag"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Contenitore di eventi utilizzato durante il salvataggio."
type: docs
weight: 65
url: /it/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

Contenitore di eventi usato durante il salvataggio di [Archive](../../com.aspose.zip/archive).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Ottiene un evento che viene sollevato prima che una voce di archivio venga compressa. |
| [getEntryCompressed()](#getEntryCompressed--) | Ottiene un evento che viene sollevato dopo che una voce di archivio è stata compressa. |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Imposta un evento che viene sollevato prima che una voce di archivio venga compressa. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | Imposta un evento che viene sollevato dopo che una voce di archivio è stata compressa. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


Ottiene un evento che viene sollevato prima che una voce di archivio venga compressa.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


Ottiene un evento che viene sollevato dopo che una voce di archivio è stata compressa.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


Imposta un evento che viene sollevato prima che una voce di archivio venga compressa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | un evento che viene sollevato prima che una voce dell'archivio venga compressa. |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


Imposta un evento che viene sollevato dopo che una voce di archivio è stata compressa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | un evento che viene sollevato dopo che una voce dell'archivio è stata compressa |

