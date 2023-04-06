---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP für .NET-API-Referenz
description: SevenZipArchiveEntry evenement. Wird ausgelöst wenn ein Teil des Rohdatenstroms komprimiert wird.
type: docs
weight: 70
url: /de/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Wird ausgelöst, wenn ein Teil des Rohdatenstroms komprimiert wird.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Bemerkungen

Ereignissender ist ein[`SevenZipArchiveEntry`](../) Beispiel.

### Beispiele

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Siehe auch

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* Montage [Aspose.Zip](../../../)


