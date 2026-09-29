---
title: "EntryEventArgs"
second_title: "Aspose.ZIP för Java API-referens"
description: "Händelseargument för händelser relaterade till poster."
type: docs
weight: 62
url: /sv/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

Händelseargument för händelser relaterade till poster.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | Initierar en ny instans av klassen [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getEntry()](#getEntry--) | Hämtar arkivposten som händelsen utlöses för. |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


Initierar en ny instans av klassen [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Arkivposten som händelsen utlöses för. |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


Hämtar arkivposten som händelsen utlöses för.

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
