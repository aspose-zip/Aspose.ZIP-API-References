---
title: "ProgressCancelEventArgs"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Clase para datos de evento cancelable que contiene el número de bytes procesados."
type: docs
weight: 95
url: /es/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

Clase para datos de evento cancelable que contiene el número de bytes procesados.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | Inicializa una nueva instancia de la clase [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCancel()](#getCancel--) | Obtiene un valor que indica si el evento debe cancelarse. |
| [setCancel(boolean value)](#setCancel-boolean-) | Establece un valor que indica si el evento debe cancelarse. |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


Inicializa una nueva instancia de la clase [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| proceededBytes | long | La cantidad de bytes procesados. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Obtiene un valor que indica si el evento debe cancelarse.

**Returns:**
boolean - Verdadero si el evento debe cancelarse; de lo contrario, falso.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Establece un valor que indica si el evento debe cancelarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si el evento debe cancelarse. |

