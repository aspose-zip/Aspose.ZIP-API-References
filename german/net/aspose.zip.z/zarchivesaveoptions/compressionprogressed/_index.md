---
title: "ZArchiveSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ZArchiveSaveOptions-Ereignis. Wird ausgelöst, wenn ein Teil des Rohdatenstroms komprimiert wird"
type: docs
weight: 20
url: /de/net/aspose.zip.z/zarchivesaveoptions/compressionprogressed/
---
## ZArchiveSaveOptions.CompressionProgressed event

Wird ausgelöst, wenn ein Teil des Rohstroms komprimiert wird.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Beispiele

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Siehe auch

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveSaveOptions](../)
* namespace [Aspose.Zip.Z](../../zarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


