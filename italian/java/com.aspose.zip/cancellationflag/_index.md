---
title: "CancellationFlag"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Il flag che consente l'annullamento delle operazioni."
type: docs
weight: 54
url: /it/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

Il flag che consente l'annullamento delle operazioni.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | Crea un'istanza di CancellationFlag. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [cancel()](#cancel--) | Annulla l'operazione associata a questa istanza di [CancellationFlag](../../com.aspose.zip/cancellationflag). |
| [cancelAfter(long delay)](#cancelAfter-long-) | Annulla l'operazione dopo un ritardo specificato in millisecondi. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | Annulla l'operazione dopo un ritardo specificato nell'unità di tempo fornita. |
| [close()](#close--) | Chiude l'istanza di [CancellationFlag](../../com.aspose.zip/cancellationflag) e rilascia tutte le risorse associate. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


Crea un'istanza di CancellationFlag.

### cancel() {#cancel--}
```
public void cancel()
```


Annulla l'operazione associata a questa istanza di [CancellationFlag](../../com.aspose.zip/cancellationflag).

Se l'operazione è già annullata, questo metodo non fa nulla.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


Annulla l'operazione dopo un ritardo specificato in millisecondi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| delay | long | Il ritardo in millisecondi dopo il quale l'operazione sarà annullata. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


Annulla l'operazione dopo un ritardo specificato nell'unità di tempo fornita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| delay | long | Il ritardo dopo il quale l'operazione sarà annullata. |
| unità | java.util.concurrent.TimeUnit | L'unità di tempo del parametro di ritardo. |

### close() {#close--}
```
public void close()
```


Chiude l'istanza di [CancellationFlag](../../com.aspose.zip/cancellationflag) e rilascia tutte le risorse associate.

