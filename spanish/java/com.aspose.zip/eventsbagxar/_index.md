---
title: "EventsBagXar"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Contenedor de eventos utilizado al guardar."
type: docs
weight: 67
url: /es/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

Contenedor de eventos utilizado al guardar [XarArchive](../../com.aspose.zip/xararchive).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Obtiene un evento que se dispara antes de que una entrada del archivo sea comprimida. |
| [getEntryCompressed()](#getEntryCompressed--) | Obtiene un evento que se dispara después de que una entrada del archivo haya sido comprimida. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | Establece un evento que se dispara antes de que una entrada del archivo sea comprimida. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | Establece un evento que se dispara después de que una entrada del archivo haya sido comprimida. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


Obtiene un evento que se dispara antes de que una entrada del archivo sea comprimida.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


Obtiene un evento que se dispara después de que una entrada del archivo haya sido comprimida.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


Establece un evento que se dispara antes de que una entrada del archivo sea comprimida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | un evento que se genera antes de que una entrada del archivo sea comprimida. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


Establece un evento que se dispara después de que una entrada del archivo haya sido comprimida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | un evento que se genera después de que una entrada del archivo ha sido comprimida |

