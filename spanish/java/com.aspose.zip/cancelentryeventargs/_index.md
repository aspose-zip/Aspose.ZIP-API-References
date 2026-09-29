---
title: "CancelEntryEventArgs"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Argumentos de evento para eventos relacionados con entradas cancelables."
type: docs
weight: 52
url: /es/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

Argumentos de evento para eventos relacionados con entradas cancelables.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | Inicializa una nueva instancia de la clase [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCancel()](#getCancel--) | Obtiene un valor que indica si el evento debe cancelarse. |
| [setCancel(boolean value)](#setCancel-boolean-) | Establece un valor que indica si el evento debe cancelarse. |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


Inicializa una nueva instancia de la clase [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Entrada del archivo para la que se genera el evento. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Obtiene un valor que indica si el evento debe cancelarse.

**Returns:**
boolean - verdadero si el evento debe cancelarse; de lo contrario, falso.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Establece un valor que indica si el evento debe cancelarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | verdadero si el evento debe cancelarse; de lo contrario, falso. |

