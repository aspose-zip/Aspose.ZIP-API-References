---
title: "CancelEntryEventArgsXar"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Arguments d'événement pour les événements liés aux entrées annulables."
type: docs
weight: 53
url: /fr/java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

Arguments d'événement pour les événements liés aux entrées annulables.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | Initialise une nouvelle instance de la classe [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCancel()](#getCancel--) | Obtient une valeur indiquant si l'événement doit être annulé. |
| [setCancel(boolean value)](#setCancel-boolean-) | Définit une valeur indiquant si l'événement doit être annulé. |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


Initialise une nouvelle instance de la classe [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | entrée d'archive pour laquelle l'événement est déclenché |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Obtient une valeur indiquant si l'événement doit être annulé.

**Returns:**
booléen - vrai si l'événement doit être annulé; sinon, faux
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Définit une valeur indiquant si l'événement doit être annulé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | vrai si l'événement doit être annulé; sinon, faux |

