---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "LzmaArchiveSettings γεγονός. Ενεργοποιείται όταν ένα τμήμα του ακατέργαστου ρεύματος συμπιέζεται"
type: docs
weight: 50
url: /el/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής συμπιέζεται.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Παραδείγματα

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


