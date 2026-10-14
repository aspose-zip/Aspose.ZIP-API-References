---
title: "XarFileEntry.CompressionProgressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "XarFileEntry händelse. Utlöses när en del av råströmmen har komprimerats"
type: docs
weight: 20
url: /sv/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

Utlöser när en del av den råa strömmen komprimeras.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Anmärkningar

Avsändaren av händelsen är en [`XarFileEntry`](../)‑instans.

## Exempel

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Se även

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


