---
title: "SevenZipArchiveEntry.CompressionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Γεγονός SevenZipArchiveEntry. Ενεργοποιείται όταν ένα τμήμα του ακατέργαστου ρεύματος συμπιέζεται"
type: docs
weight: 70
url: /el/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής συμπιέζεται.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Παρατηρήσεις

Ο αποστολέας του γεγονότος είναι μια παρουσία του [`SevenZipArchiveEntry`](../).

Δεν καλείται σε λειτουργία solid και σε πολυνηματική λειτουργία για καταχωρήσεις LZMA2.

## Παραδείγματα

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assembly [Aspose.Zip](../../../)


