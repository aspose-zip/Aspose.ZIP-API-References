---
title: "EventsBag"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Contenedor de eventos utilizado al guardar."
type: docs
weight: 65
url: /es/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

Contenedor de eventos usado al guardar [Archive](../../com.aspose.zip/archive).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Obtiene un evento que se dispara antes de que una entrada del archivo sea comprimida. |
| [getEntryCompressed()](#getEntryCompressed--) | Obtiene un evento que se dispara después de que una entrada del archivo haya sido comprimida. |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Establece un evento que se dispara antes de que una entrada del archivo sea comprimida. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | Establece un evento que se dispara después de que una entrada del archivo haya sido comprimida. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


Obtiene un evento que se dispara antes de que una entrada del archivo sea comprimida.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


Obtiene un evento que se dispara después de que una entrada del archivo haya sido comprimida.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


Establece un evento que se dispara antes de que una entrada del archivo sea comprimida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | un evento que se genera antes de que una entrada del archivo sea comprimida. |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


Establece un evento que se dispara después de que una entrada del archivo haya sido comprimida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | un evento que se genera después de que una entrada del archivo ha sido comprimida |

