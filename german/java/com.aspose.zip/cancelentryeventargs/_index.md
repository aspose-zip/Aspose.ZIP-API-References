---
title: "CancelEntryEventArgs"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Ereignisargumente für abbrechbare, eintragsbezogene Ereignisse."
type: docs
weight: 52
url: /de/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

Ereignisargumente für abbrechbare, eintragsbezogene Ereignisse.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | Initialisiert eine neue Instanz der [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCancel()](#getCancel--) | Gibt einen Wert zurück, der angibt, ob das Ereignis abgebrochen werden soll. |
| [setCancel(boolean value)](#setCancel-boolean-) | Setzt einen Wert, der angibt, ob das Ereignis abgebrochen werden soll. |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


Initialisiert eine neue Instanz der [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Archiv-Eintrag, für den das Ereignis ausgelöst wird. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Gibt einen Wert zurück, der angibt, ob das Ereignis abgebrochen werden soll.

**Returns:**
boolean – true, wenn das Ereignis abgebrochen werden soll; andernfalls false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Setzt einen Wert, der angibt, ob das Ereignis abgebrochen werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | true, wenn das Ereignis abgebrochen werden soll; andernfalls false. |

