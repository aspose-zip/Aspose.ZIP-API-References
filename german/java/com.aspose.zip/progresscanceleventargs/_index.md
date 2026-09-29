---
title: "ProgressCancelEventArgs"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Klasse für abbrechbare Ereignisdaten, die die Anzahl der verarbeiteten Bytes enthält."
type: docs
weight: 95
url: /de/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

Klasse für abbrechbare Ereignisdaten, die die Anzahl der verarbeiteten Bytes enthält.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | Initialisiert eine neue Instanz der [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCancel()](#getCancel--) | Gibt einen Wert zurück, der angibt, ob das Ereignis abgebrochen werden soll. |
| [setCancel(boolean value)](#setCancel-boolean-) | Setzt einen Wert, der angibt, ob das Ereignis abgebrochen werden soll. |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


Initialisiert eine neue Instanz der [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| proceededBytes | long | Die Anzahl der verarbeiteten Bytes. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Gibt einen Wert zurück, der angibt, ob das Ereignis abgebrochen werden soll.

**Returns:**
boolean - True, wenn das Ereignis abgebrochen werden soll; andernfalls false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Setzt einen Wert, der angibt, ob das Ereignis abgebrochen werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Ein Wert, der angibt, ob das Ereignis abgebrochen werden soll. |

