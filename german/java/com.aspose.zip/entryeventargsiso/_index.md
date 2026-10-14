---
title: "EntryEventArgsIso"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Ereignisargumente für eintragsbezogene Ereignisse."
type: docs
weight: 63
url: /de/java/com.aspose.zip/entryeventargsiso/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsIso extends System.EventArgs
```

Ereignisargumente für eintragsbezogene Ereignisse.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [EntryEventArgsIso(IsoEntry entry)](#EntryEventArgsIso-com.aspose.zip.IsoEntry-) | Initialisiert eine neue Instanz der [EntryEventArgs](../../com.aspose.zip/entryeventargs)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getEntry()](#getEntry--) | Liefert den Archiveintrag, für den das Ereignis ausgelöst wird. |
### EntryEventArgsIso(IsoEntry entry) {#EntryEventArgsIso-com.aspose.zip.IsoEntry-}
```
public EntryEventArgsIso(IsoEntry entry)
```


Initialisiert eine neue Instanz der [EntryEventArgs](../../com.aspose.zip/entryeventargs)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| entry | [IsoEntry](../../com.aspose.zip/isoentry) | der Archiveintrag, für den das Ereignis ausgelöst wird |

### getEntry() {#getEntry--}
```
public final IsoEntry getEntry()
```


Liefert den Archiveintrag, für den das Ereignis ausgelöst wird.

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the archive entry the event is raised for
