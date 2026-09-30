---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "LzmaArchiveSettings händelse. Utlöses när en del av råströmmen har komprimerats"
type: docs
weight: 50
url: /sv/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

Utlöser när en del av den råa strömmen komprimeras.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Exempel

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Se även

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


