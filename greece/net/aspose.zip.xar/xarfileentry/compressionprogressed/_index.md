---
title: "XarFileEntry.CompressionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Γεγονός XarFileEntry. Ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται"
type: docs
weight: 20
url: /el/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής συμπιέζεται.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Παρατηρήσεις

Ο αποστολέας του γεγονότος είναι μια παρουσία του [`XarFileEntry`](../).

## Παραδείγματα

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


