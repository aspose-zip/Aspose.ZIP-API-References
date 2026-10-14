---
title: "EntryEventArgsXar"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Argomenti dell'evento per eventi relativi a voci."
type: docs
weight: 64
url: /it/java/com.aspose.zip/entryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsXar extends System.EventArgs
```

Argomenti dell'evento per eventi relativi a voci.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [EntryEventArgsXar(XarEntry entry)](#EntryEventArgsXar-com.aspose.zip.XarEntry-) | Inizializza una nuova istanza della classe [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getEntry()](#getEntry--) | Ottiene la voce dell'archivio per la quale viene sollevato l'evento. |
### EntryEventArgsXar(XarEntry entry) {#EntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public EntryEventArgsXar(XarEntry entry)
```


Inizializza una nuova istanza della classe [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | la voce dell'archivio per la quale viene sollevato l'evento |

### getEntry() {#getEntry--}
```
public final XarEntry getEntry()
```


Ottiene la voce dell'archivio per la quale viene sollevato l'evento.

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - the archive entry the event is raised for
