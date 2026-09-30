---
title: "ZstandardSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ZstandardSaveOptions-händelse. Utlöses när en del av råströmmen har komprimerats"
type: docs
weight: 20
url: /sv/net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

Utlöser när en del av den råa strömmen komprimeras.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Exempel

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Se även

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


