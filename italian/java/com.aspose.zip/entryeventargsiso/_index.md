---
title: "EntryEventArgsIso"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Argomenti dell'evento per eventi relativi a voci."
type: docs
weight: 63
url: /it/java/com.aspose.zip/entryeventargsiso/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsIso extends System.EventArgs
```

Argomenti dell'evento per eventi relativi a voci.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [EntryEventArgsIso(IsoEntry entry)](#EntryEventArgsIso-com.aspose.zip.IsoEntry-) | Inizializza una nuova istanza della classe [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getEntry()](#getEntry--) | Ottiene la voce dell'archivio per la quale viene sollevato l'evento. |
### EntryEventArgsIso(IsoEntry entry) {#EntryEventArgsIso-com.aspose.zip.IsoEntry-}
```
public EntryEventArgsIso(IsoEntry entry)
```


Inizializza una nuova istanza della classe [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| entry | [IsoEntry](../../com.aspose.zip/isoentry) | la voce dell'archivio per la quale viene sollevato l'evento |

### getEntry() {#getEntry--}
```
public final IsoEntry getEntry()
```


Ottiene la voce dell'archivio per la quale viene sollevato l'evento.

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the archive entry the event is raised for
