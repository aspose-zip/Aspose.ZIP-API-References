---
title: "ZArchiveSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ZArchiveSaveOptions gebeurtenis. Wordt geactiveerd wanneer een deel van de ruwe stream is gecomprimeerd"
type: docs
weight: 20
url: /nl/net/aspose.zip.z/zarchivesaveoptions/compressionprogressed/
---
## ZArchiveSaveOptions.CompressionProgressed event

Wordt opgegooid wanneer een deel van de ruwe stream wordt gecomprimeerd.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Voorbeelden

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Zie ook

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveSaveOptions](../)
* namespace [Aspose.Zip.Z](../../zarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


