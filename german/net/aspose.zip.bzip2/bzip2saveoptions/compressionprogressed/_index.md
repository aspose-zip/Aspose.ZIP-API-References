---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Bzip2SaveOptions-Ereignis. Wird ausgelöst, wenn ein Teil des Rohstreams komprimiert wird"
type: docs
weight: 40
url: /de/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

Wird ausgelöst, wenn ein Teil des Rohstroms komprimiert wird.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Hinweise

Dieses Ereignis wird im Mehrthread-Modus beim Komprimieren nicht ausgelöst.

## Beispiele

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Siehe auch

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


