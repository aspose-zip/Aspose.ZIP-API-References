---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Γεγονός Bzip2SaveOptions. Ενεργοποιείται όταν συμπιέζεται ένα τμήμα ακατέργαστου ρεύματος."
type: docs
weight: 40
url: /el/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής συμπιέζεται.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Παρατηρήσεις

Αυτό το γεγονός δεν θα ενεργοποιηθεί όταν γίνεται συμπίεση σε πολυνηματική λειτουργία.

## Παραδείγματα

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


