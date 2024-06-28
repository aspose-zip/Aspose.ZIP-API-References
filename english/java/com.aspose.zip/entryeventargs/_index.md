---
title: EntryEventArgs
second_title: Aspose.ZIP for Java API Reference
description: Event arguments for entry related events.
type: docs
weight: 33
url: /java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

Event arguments for entry related events.
## Constructors

| Constructor | Description |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | Initializes a new instance of the [EntryEventArgs](../../com.aspose.zip/entryeventargs) class. |
## Methods

| Method | Description |
| --- | --- |
| [getEntry()](#getEntry--) | Gets the archive entry the event is raised for. |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


Initializes a new instance of the [EntryEventArgs](../../com.aspose.zip/entryeventargs) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Archive entry the event is raised for. |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


Gets the archive entry the event is raised for.

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
