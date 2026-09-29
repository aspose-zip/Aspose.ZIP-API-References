---
title: "CancelEntryEventArgsXar"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Argumentos de evento para eventos relacionados con entradas cancelables."
type: docs
weight: 53
url: /es/java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

Argumentos de evento para eventos relacionados con entradas cancelables.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | Inicializa una nueva instancia de la clase [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCancel()](#getCancel--) | Obtiene un valor que indica si el evento debe cancelarse. |
| [setCancel(boolean value)](#setCancel-boolean-) | Establece un valor que indica si el evento debe cancelarse. |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


Inicializa una nueva instancia de la clase [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | entrada del archivo para la cual se genera el evento |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Obtiene un valor que indica si el evento debe cancelarse.

**Returns:**
boolean - true si el evento debe cancelarse; de lo contrario, false
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Establece un valor que indica si el evento debe cancelarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | true si el evento debe cancelarse; de lo contrario, false |

