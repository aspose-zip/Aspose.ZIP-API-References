---
title: "CancelEntryEventArgs"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Argomenti dell'evento per eventi relativi a voci annullabili."
type: docs
weight: 52
url: /it/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

Argomenti dell'evento per eventi relativi a voci annullabili.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | Inizializza una nuova istanza della classe [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCancel()](#getCancel--) | Restituisce un valore che indica se l'evento deve essere annullato. |
| [setCancel(boolean value)](#setCancel-boolean-) | Imposta un valore che indica se l'evento deve essere annullato. |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


Inizializza una nuova istanza della classe [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Voce dell'archivio per la quale viene sollevato l'evento. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Restituisce un valore che indica se l'evento deve essere annullato.

**Returns:**
boolean - true se l'evento deve essere annullato; altrimenti, false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Imposta un valore che indica se l'evento deve essere annullato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | true se l'evento deve essere annullato; altrimenti, false. |

