---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP för .NET API-referens
description: SevenZipArchiveEntry händelse. Ökar när en del av råströmmen komprimeras.
type: docs
weight: 70
url: /sv/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Ökar när en del av råströmmen komprimeras.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Anmärkningar

Händelseavsändaren är en[`SevenZipArchiveEntry`](../) exempel.

### Exempel

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Se även

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* hopsättning [Aspose.Zip](../../../)


