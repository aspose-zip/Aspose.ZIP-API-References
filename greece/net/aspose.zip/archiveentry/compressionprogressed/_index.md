---
title: ArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP για Αναφορά API .NET
description: ArchiveEntry Εκδήλωση. Αυξάνεται όταν συμπιέζεται ένα τμήμα της ακατέργαστης ροής.
type: docs
weight: 80
url: /el/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Αυξάνεται όταν συμπιέζεται ένα τμήμα της ακατέργαστης ροής.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Παρατηρήσεις

Ο αποστολέας συμβάντος είναι ένας[`ArchiveEntry`](../) παράδειγμα.

### Παραδείγματα

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Δείτε επίσης

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* χώρος ονομάτων [Aspose.Zip](../../archiveentry/)
* συνέλευση [Aspose.Zip](../../../)


