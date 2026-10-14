---
title: "EventsBagIso"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Contenedor de eventos utilizado al guardar."
type: docs
weight: 66
url: /es/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

Contenedor de eventos utilizado al guardar [IsoArchive](../../com.aspose.zip/isoarchive).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Obtiene un evento que se dispara antes de que una entrada del archivo sea comprimida. |
| [getEntryCompressed()](#getEntryCompressed--) | Obtiene un evento que se dispara después de que una entrada del archivo haya sido comprimida. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Establece un evento que se dispara antes de que una entrada del archivo sea comprimida. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Establece un evento que se dispara después de que una entrada del archivo haya sido comprimida. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


Obtiene un evento que se dispara antes de que una entrada del archivo sea comprimida.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


Obtiene un evento que se dispara después de que una entrada del archivo haya sido comprimida.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


Establece un evento que se dispara antes de que una entrada del archivo sea comprimida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | un evento que se genera antes de que una entrada del archivo sea comprimida. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


Establece un evento que se dispara después de que una entrada del archivo haya sido comprimida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | un evento que se genera después de que una entrada del archivo ha sido comprimida |

