---
title: "ZstandardSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "ZstandardSaveOptions event. Ενεργοποιείται όταν ένα τμήμα του ακατέργαστου ρεύματος συμπιέζεται"
type: docs
weight: 20
url: /el/net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής συμπιέζεται.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Παραδείγματα

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


