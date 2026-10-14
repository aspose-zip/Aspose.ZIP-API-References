---
title: "EntryEventArgsXar"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Ereignisargumente für eintragsbezogene Ereignisse."
type: docs
weight: 64
url: /de/java/com.aspose.zip/entryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsXar extends System.EventArgs
```

Ereignisargumente für eintragsbezogene Ereignisse.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [EntryEventArgsXar(XarEntry entry)](#EntryEventArgsXar-com.aspose.zip.XarEntry-) | Initialisiert eine neue Instanz der [EntryEventArgs](../../com.aspose.zip/entryeventargs)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getEntry()](#getEntry--) | Liefert den Archiveintrag, für den das Ereignis ausgelöst wird. |
### EntryEventArgsXar(XarEntry entry) {#EntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public EntryEventArgsXar(XarEntry entry)
```


Initialisiert eine neue Instanz der [EntryEventArgs](../../com.aspose.zip/entryeventargs)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | der Archiveintrag, für den das Ereignis ausgelöst wird |

### getEntry() {#getEntry--}
```
public final XarEntry getEntry()
```


Liefert den Archiveintrag, für den das Ereignis ausgelöst wird.

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - the archive entry the event is raised for
