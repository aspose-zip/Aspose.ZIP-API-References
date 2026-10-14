---
title: "ZArchiveSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Συμβάν ZArchiveSaveOptions. Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής συμπιέζεται"
type: docs
weight: 20
url: /el/net/aspose.zip.z/zarchivesaveoptions/compressionprogressed/
---
## ZArchiveSaveOptions.CompressionProgressed event

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
* class [ZArchiveSaveOptions](../)
* namespace [Aspose.Zip.Z](../../zarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


