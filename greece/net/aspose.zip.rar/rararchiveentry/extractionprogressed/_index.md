---
title: RarArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP για Αναφορά API .NET
description: RarArchiveEntry Εκδήλωση. Αυξάνεται όταν εξάγεται ένα τμήμα της ακατέργαστης ροής.
type: docs
weight: 80
url: /el/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Αυξάνεται όταν εξάγεται ένα τμήμα της ακατέργαστης ροής.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Παρατηρήσεις

Ο αποστολέας συμβάντος είναι ένας[`RarArchiveEntry`](../) παράδειγμα.

### Παραδείγματα

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* χώρος ονομάτων [Aspose.Zip.Rar](../../rararchiveentry/)
* συνέλευση [Aspose.Zip](../../../)


