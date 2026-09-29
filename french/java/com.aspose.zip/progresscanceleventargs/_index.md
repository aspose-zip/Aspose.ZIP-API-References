---
title: "ProgressCancelEventArgs"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Classe pour les données d'événement annulables contenant le nombre d'octets traités."
type: docs
weight: 95
url: /fr/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

Classe pour les données d'événement annulables contenant le nombre d'octets traités.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | Initialise une nouvelle instance de la classe [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCancel()](#getCancel--) | Obtient une valeur indiquant si l'événement doit être annulé. |
| [setCancel(boolean value)](#setCancel-boolean-) | Définit une valeur indiquant si l'événement doit être annulé. |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


Initialise une nouvelle instance de la classe [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| proceededBytes | long | Le nombre d'octets traités. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Obtient une valeur indiquant si l'événement doit être annulé.

**Returns:**
booléen - Vrai si l'événement doit être annulé; sinon, faux.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Définit une valeur indiquant si l'événement doit être annulé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si l'événement doit être annulé. |

