---
title: "EntryEventArgs"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Ereignisargumente für eintragsbezogene Ereignisse."
type: docs
weight: 62
url: /de/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

Ereignisargumente für eintragsbezogene Ereignisse.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | Initialisiert eine neue Instanz der [EntryEventArgs](../../com.aspose.zip/entryeventargs)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getEntry()](#getEntry--) | Liefert den Archiveintrag, für den das Ereignis ausgelöst wird. |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


Initialisiert eine neue Instanz der [EntryEventArgs](../../com.aspose.zip/entryeventargs)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Archiv-Eintrag, für den das Ereignis ausgelöst wird. |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


Liefert den Archiveintrag, für den das Ereignis ausgelöst wird.

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
