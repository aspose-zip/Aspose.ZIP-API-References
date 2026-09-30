---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Γεγονός Bzip2LoadOptions. Το γεγονός ενεργοποιείται όταν έχουν εξαχθεί ορισμένα byte."
type: docs
weight: 30
url: /el/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

Γεγονός που ενεργοποιείται όταν έχουν εξαχθεί ορισμένα bytes.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Παρατηρήσεις

Ο αποστολέας του γεγονότος είναι η παρουσία [`Bzip2Archive`](../../bzip2archive/) της οποίας η εξαγωγή προχωρά. Το [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) είναι ο αριθμός των byte μετά την εξαγωγή.

## Παραδείγματα

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


