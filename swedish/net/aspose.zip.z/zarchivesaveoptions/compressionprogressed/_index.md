---
title: "ZArchiveSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ZArchiveSaveOptions händelse. Utlöser när en del av den råa strömmen har komprimerats"
type: docs
weight: 20
url: /sv/net/aspose.zip.z/zarchivesaveoptions/compressionprogressed/
---
## ZArchiveSaveOptions.CompressionProgressed event

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
* class [ZArchiveSaveOptions](../)
* namespace [Aspose.Zip.Z](../../zarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


