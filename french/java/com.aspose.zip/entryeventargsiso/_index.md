---
title: "EntryEventArgsIso"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Arguments d'événement pour les événements liés aux entrées."
type: docs
weight: 63
url: /fr/java/com.aspose.zip/entryeventargsiso/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsIso extends System.EventArgs
```

Arguments d'événement pour les événements liés aux entrées.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [EntryEventArgsIso(IsoEntry entry)](#EntryEventArgsIso-com.aspose.zip.IsoEntry-) | Initialise une nouvelle instance de la classe [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getEntry()](#getEntry--) | Obtient l'entrée d'archive pour laquelle l'événement est déclenché. |
### EntryEventArgsIso(IsoEntry entry) {#EntryEventArgsIso-com.aspose.zip.IsoEntry-}
```
public EntryEventArgsIso(IsoEntry entry)
```


Initialise une nouvelle instance de la classe [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| entry | [IsoEntry](../../com.aspose.zip/isoentry) | l'entrée d'archive pour laquelle l'événement est déclenché |

### getEntry() {#getEntry--}
```
public final IsoEntry getEntry()
```


Obtient l'entrée d'archive pour laquelle l'événement est déclenché.

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the archive entry the event is raised for
