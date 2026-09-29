---
title: "EntryEventArgsIso"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Argumentos de evento para eventos relacionados con entradas."
type: docs
weight: 63
url: /es/java/com.aspose.zip/entryeventargsiso/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsIso extends System.EventArgs
```

Argumentos de evento para eventos relacionados con entradas.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [EntryEventArgsIso(IsoEntry entry)](#EntryEventArgsIso-com.aspose.zip.IsoEntry-) | Inicializa una nueva instancia de la clase [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getEntry()](#getEntry--) | Obtiene la entrada del archivo para la cual se genera el evento. |
### EntryEventArgsIso(IsoEntry entry) {#EntryEventArgsIso-com.aspose.zip.IsoEntry-}
```
public EntryEventArgsIso(IsoEntry entry)
```


Inicializa una nueva instancia de la clase [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| entry | [IsoEntry](../../com.aspose.zip/isoentry) | la entrada del archivo para la cual se genera el evento |

### getEntry() {#getEntry--}
```
public final IsoEntry getEntry()
```


Obtiene la entrada del archivo para la cual se genera el evento.

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the archive entry the event is raised for
