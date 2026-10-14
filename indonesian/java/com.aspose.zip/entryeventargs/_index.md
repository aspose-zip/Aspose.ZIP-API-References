---
title: "EntryEventArgs"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Argumen peristiwa untuk peristiwa terkait entri."
type: docs
weight: 62
url: /id/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

Argumen peristiwa untuk peristiwa terkait entri.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | Menginisialisasi instance baru dari kelas [EntryEventArgs](../../com.aspose.zip/entryeventargs) class. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getEntry()](#getEntry--) | Mendapatkan entri arsip yang memicu acara. |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


Menginisialisasi instance baru dari kelas [EntryEventArgs](../../com.aspose.zip/entryeventargs) class.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Entri arsip yang memicu acara ini. |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


Mendapatkan entri arsip yang memicu acara.

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
