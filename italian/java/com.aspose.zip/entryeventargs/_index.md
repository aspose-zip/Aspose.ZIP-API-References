---
title: "EntryEventArgs"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Argomenti dell'evento per eventi relativi a voci."
type: docs
weight: 62
url: /it/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

Argomenti dell'evento per eventi relativi a voci.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | Inizializza una nuova istanza della classe [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getEntry()](#getEntry--) | Ottiene la voce dell'archivio per la quale viene sollevato l'evento. |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


Inizializza una nuova istanza della classe [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Voce dell'archivio per la quale viene sollevato l'evento. |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


Ottiene la voce dell'archivio per la quale viene sollevato l'evento.

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
