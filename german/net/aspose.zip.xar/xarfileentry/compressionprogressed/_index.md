---
title: "XarFileEntry.CompressionProgressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "XarFileEntry Ereignis. Wird ausgelöst, wenn ein Teil des Rohdatenstroms komprimiert wird."
type: docs
weight: 20
url: /de/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

Wird ausgelöst, wenn ein Teil des Rohstroms komprimiert wird.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Hinweise

Der Ereignisabsender ist eine [`XarFileEntry`](../) Instanz.

## Beispiele

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Siehe auch

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


