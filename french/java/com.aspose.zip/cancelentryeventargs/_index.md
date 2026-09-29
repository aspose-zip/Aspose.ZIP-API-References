---
title: "CancelEntryEventArgs"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Arguments d'événement pour les événements liés aux entrées annulables."
type: docs
weight: 52
url: /fr/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

Arguments d'événement pour les événements liés aux entrées annulables.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | Initialise une nouvelle instance de la classe [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCancel()](#getCancel--) | Obtient une valeur indiquant si l'événement doit être annulé. |
| [setCancel(boolean value)](#setCancel-boolean-) | Définit une valeur indiquant si l'événement doit être annulé. |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


Initialise une nouvelle instance de la classe [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Entrée d'archive pour laquelle l'événement est déclenché. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Obtient une valeur indiquant si l'événement doit être annulé.

**Returns:**
boolean - true si l'événement doit être annulé ; sinon, false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Définit une valeur indiquant si l'événement doit être annulé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | true si l'événement doit être annulé ; sinon, false. |

