---
title: "EntryEventArgs"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Evenementargumenten voor itemgerelateerde gebeurtenissen."
type: docs
weight: 62
url: /nl/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

Evenementargumenten voor itemgerelateerde gebeurtenissen.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | Initialiseert een nieuw exemplaar van de [EntryEventArgs](../../com.aspose.zip/entryeventargs) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getEntry()](#getEntry--) | Haalt het archiefitem op waarvoor het evenement wordt getriggerd. |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


Initialiseert een nieuw exemplaar van de [EntryEventArgs](../../com.aspose.zip/entryeventargs) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Archiefitem waarvoor het evenement wordt opgehaald. |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


Haalt het archiefitem op waarvoor het evenement wordt getriggerd.

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
