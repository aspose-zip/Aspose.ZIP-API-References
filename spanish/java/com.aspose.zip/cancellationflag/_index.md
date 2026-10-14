---
title: "CancellationFlag"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "La bandera que permite la cancelación de operaciones."
type: docs
weight: 54
url: /es/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

La bandera que permite la cancelación de operaciones.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | Construye una instancia de CancellationFlag. |
## Métodos

| Método | Descripción |
| --- | --- |
| [cancel()](#cancel--) | Cancela la operación asociada con esta instancia de [CancellationFlag](../../com.aspose.zip/cancellationflag). |
| [cancelAfter(long delay)](#cancelAfter-long-) | Cancela la operación después de un retraso especificado en milisegundos. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | Cancela la operación después de un retraso especificado en la unidad de tiempo dada. |
| [close()](#close--) | Cierra la instancia de [CancellationFlag](../../com.aspose.zip/cancellationflag) y libera cualquier recurso asociado con ella. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


Construye una instancia de CancellationFlag.

### cancel() {#cancel--}
```
public void cancel()
```


Cancela la operación asociada con esta instancia de [CancellationFlag](../../com.aspose.zip/cancellationflag).

Si la operación ya está cancelada, este método no hace nada.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


Cancela la operación después de un retraso especificado en milisegundos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| delay | long | El retraso en milisegundos después del cual la operación será cancelada. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


Cancela la operación después de un retraso especificado en la unidad de tiempo dada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| delay | long | El retraso después del cual la operación será cancelada. |
| unit | java.util.concurrent.TimeUnit | La unidad de tiempo del parámetro de retardo. |

### close() {#close--}
```
public void close()
```


Cierra la instancia de [CancellationFlag](../../com.aspose.zip/cancellationflag) y libera cualquier recurso asociado con ella.

