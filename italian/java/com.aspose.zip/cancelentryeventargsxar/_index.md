---
title: "CancelEntryEventArgsXar"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Argomenti dell'evento per eventi relativi a voci annullabili."
type: docs
weight: 53
url: /it/java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

Argomenti dell'evento per eventi relativi a voci annullabili.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | Inizializza una nuova istanza della classe [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCancel()](#getCancel--) | Restituisce un valore che indica se l'evento deve essere annullato. |
| [setCancel(boolean value)](#setCancel-boolean-) | Imposta un valore che indica se l'evento deve essere annullato. |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


Inizializza una nuova istanza della classe [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | voce dell'archivio per cui viene sollevato l'evento |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Restituisce un valore che indica se l'evento deve essere annullato.

**Returns:**
boolean - true se l'evento deve essere annullato; altrimenti, false
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Imposta un valore che indica se l'evento deve essere annullato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | true se l'evento deve essere annullato; altrimenti, false |

