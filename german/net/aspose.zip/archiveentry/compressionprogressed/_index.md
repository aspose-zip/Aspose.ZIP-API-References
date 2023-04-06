---
title: ArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP für .NET-API-Referenz
description: ArchiveEntry evenement. Wird ausgelöst wenn ein Teil des Rohdatenstroms komprimiert wird.
type: docs
weight: 80
url: /de/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Wird ausgelöst, wenn ein Teil des Rohdatenstroms komprimiert wird.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Bemerkungen

Ereignissender ist ein[`ArchiveEntry`](../) Beispiel.

### Beispiele

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Siehe auch

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* namensraum [Aspose.Zip](../../archiveentry/)
* Montage [Aspose.Zip](../../../)


