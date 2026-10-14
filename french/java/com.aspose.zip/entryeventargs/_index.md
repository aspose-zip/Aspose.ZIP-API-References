---
title: "EntryEventArgs"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Arguments d'événement pour les événements liés aux entrées."
type: docs
weight: 62
url: /fr/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

Arguments d'événement pour les événements liés aux entrées.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | Initialise une nouvelle instance de la classe [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getEntry()](#getEntry--) | Obtient l'entrée d'archive pour laquelle l'événement est déclenché. |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


Initialise une nouvelle instance de la classe [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Entrée d'archive pour laquelle l'événement est déclenché. |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


Obtient l'entrée d'archive pour laquelle l'événement est déclenché.

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
