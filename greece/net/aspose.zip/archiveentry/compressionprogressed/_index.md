---
title: "ArchiveEntry.CompressionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Συμβάν ArchiveEntry. Ενεργοποιείται όταν ένα τμήμα του ακατέργαστου ρεύματος συμπιέζεται"
type: docs
weight: 90
url: /el/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής συμπιέζεται.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Παρατηρήσεις

Ο αποστολέας του συμβάντος είναι μια παρουσία του [`ArchiveEntry`](../).

## Παραδείγματα

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Δείτε επίσης

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


