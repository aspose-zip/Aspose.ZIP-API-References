---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Γεγονός ZArchiveLoadOptions. Λαμβάνει ή ορίζει τον delegate που καλείται όταν έχουν εξαχθεί κάποια bytes"
type: docs
weight: 30
url: /el/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

Λαμβάνει ή ορίζει τον αντιπρόσωπο που καλείται όταν έχουν εξαχθεί κάποια byte.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Παρατηρήσεις

Ο αποστολέας του γεγονότος είναι το αντικείμενο [`ZArchive`](../../zarchive/) του οποίου η εξαγωγή προχωρά.

## Παραδείγματα

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


