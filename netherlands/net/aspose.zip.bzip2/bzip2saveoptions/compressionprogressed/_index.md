---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Bzip2SaveOptions gebeurtenis. Wordt geactiveerd wanneer een deel van de ruwe stream is gecomprimeerd"
type: docs
weight: 40
url: /nl/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

Wordt opgegooid wanneer een deel van de ruwe stream wordt gecomprimeerd.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Opmerkingen

Deze gebeurtenis wordt niet geactiveerd bij compressie in multithreaded-modus.

## Voorbeelden

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Zie ook

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


