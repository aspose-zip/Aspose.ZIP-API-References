---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP για Αναφορά API .NET
description: SevenZipArchiveEntry Εκδήλωση. Αυξάνεται όταν συμπιέζεται ένα τμήμα της ακατέργαστης ροής.
type: docs
weight: 70
url: /el/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Αυξάνεται όταν συμπιέζεται ένα τμήμα της ακατέργαστης ροής.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Παρατηρήσεις

Ο αποστολέας συμβάντος είναι ένας[`SevenZipArchiveEntry`](../) παράδειγμα.

### Παραδείγματα

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* συνέλευση [Aspose.Zip](../../../)


