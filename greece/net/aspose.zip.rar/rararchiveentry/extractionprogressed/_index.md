---
title: "RarArchiveEntry.ExtractionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Γεγονός RarArchiveEntry. Ενεργοποιείται όταν εξάγεται ένα τμήμα του ακατέργαστου ρεύματος"
type: docs
weight: 80
url: /el/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής εξάγεται.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Παρατηρήσεις

Ο αποστολέας του γεγονότος είναι μια παρουσία του [`RarArchiveEntry`](../).

## Παραδείγματα

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)


