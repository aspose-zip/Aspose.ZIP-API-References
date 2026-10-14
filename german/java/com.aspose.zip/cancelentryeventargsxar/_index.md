---
title: "CancelEntryEventArgsXar"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Ereignisargumente für abbrechbare, eintragsbezogene Ereignisse."
type: docs
weight: 53
url: /de/java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

Ereignisargumente für abbrechbare, eintragsbezogene Ereignisse.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | Initialisiert eine neue Instanz der [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCancel()](#getCancel--) | Gibt einen Wert zurück, der angibt, ob das Ereignis abgebrochen werden soll. |
| [setCancel(boolean value)](#setCancel-boolean-) | Setzt einen Wert, der angibt, ob das Ereignis abgebrochen werden soll. |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


Initialisiert eine neue Instanz der [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | Archiv-Eintrag, für den das Ereignis ausgelöst wird |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Gibt einen Wert zurück, der angibt, ob das Ereignis abgebrochen werden soll.

**Returns:**
boolean - true, wenn das Ereignis abgebrochen werden soll; andernfalls false
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Setzt einen Wert, der angibt, ob das Ereignis abgebrochen werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | true, wenn das Ereignis abgebrochen werden soll; andernfalls false |

