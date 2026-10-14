---
title: "EntryEventArgs"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Παράμετροι συμβάντος για συμβάντα σχετιζόμενα με καταχώρηση."
type: docs
weight: 62
url: /el/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

Παράμετροι συμβάντος για συμβάντα σχετιζόμενα με καταχώρηση.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [EntryEventArgs](../../com.aspose.zip/entryeventargs). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getEntry()](#getEntry--) | Λαμβάνει την καταχώρηση του αρχείου για την οποία ενεργοποιείται το συμβάν. |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [EntryEventArgs](../../com.aspose.zip/entryeventargs).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Καταχώρηση αρχείου για την οποία ενεργοποιείται το γεγονός. |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


Λαμβάνει την καταχώρηση του αρχείου για την οποία ενεργοποιείται το συμβάν.

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
