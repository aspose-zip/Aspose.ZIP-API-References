---
title: "ProgressCancelEventArgs"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Classe per i dati dell'evento annullabile contenente il numero di byte elaborati."
type: docs
weight: 95
url: /it/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

Classe per i dati dell'evento annullabile contenente il numero di byte elaborati.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | Inizializza una nuova istanza della classe [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCancel()](#getCancel--) | Restituisce un valore che indica se l'evento deve essere annullato. |
| [setCancel(boolean value)](#setCancel-boolean-) | Imposta un valore che indica se l'evento deve essere annullato. |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


Inizializza una nuova istanza della classe [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| proceededBytes | long | Il numero di byte elaborati. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Restituisce un valore che indica se l'evento deve essere annullato.

**Returns:**
boolean - True se l'evento deve essere annullato; altrimenti, false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Imposta un valore che indica se l'evento deve essere annullato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se l'evento deve essere annullato. |

