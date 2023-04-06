---
title: ArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP για Αναφορά API .NET
description: ArchiveEntry Εκδήλωση. Αυξάνεται όταν εξάγεται ένα τμήμα της ακατέργαστης ροής.
type: docs
weight: 90
url: /el/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Αυξάνεται όταν εξάγεται ένα τμήμα της ακατέργαστης ροής.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Παρατηρήσεις

Ο αποστολέας συμβάντος είναι ένας[`ArchiveEntry`](../) παράδειγμα.

### Παραδείγματα

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### Δείτε επίσης

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* χώρος ονομάτων [Aspose.Zip](../../archiveentry/)
* συνέλευση [Aspose.Zip](../../../)


