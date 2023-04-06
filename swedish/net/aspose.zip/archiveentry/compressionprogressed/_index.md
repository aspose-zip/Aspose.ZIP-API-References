---
title: ArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP för .NET API-referens
description: ArchiveEntry händelse. Ökar när en del av råströmmen komprimeras.
type: docs
weight: 80
url: /sv/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Ökar när en del av råströmmen komprimeras.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Anmärkningar

Händelseavsändaren är en[`ArchiveEntry`](../) exempel.

### Exempel

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Se även

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* namnutrymme [Aspose.Zip](../../archiveentry/)
* hopsättning [Aspose.Zip](../../../)


