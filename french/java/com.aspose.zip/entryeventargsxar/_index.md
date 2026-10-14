---
title: "EntryEventArgsXar"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Arguments d'événement pour les événements liés aux entrées."
type: docs
weight: 64
url: /fr/java/com.aspose.zip/entryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsXar extends System.EventArgs
```

Arguments d'événement pour les événements liés aux entrées.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [EntryEventArgsXar(XarEntry entry)](#EntryEventArgsXar-com.aspose.zip.XarEntry-) | Initialise une nouvelle instance de la classe [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getEntry()](#getEntry--) | Obtient l'entrée d'archive pour laquelle l'événement est déclenché. |
### EntryEventArgsXar(XarEntry entry) {#EntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public EntryEventArgsXar(XarEntry entry)
```


Initialise une nouvelle instance de la classe [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | l'entrée d'archive pour laquelle l'événement est déclenché |

### getEntry() {#getEntry--}
```
public final XarEntry getEntry()
```


Obtient l'entrée d'archive pour laquelle l'événement est déclenché.

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - the archive entry the event is raised for
