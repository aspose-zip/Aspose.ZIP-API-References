---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "ZstandardLoadOptions event. Λαμβάνει ή ορίζει τον delegate που καλείται όταν έχουν εξαχθεί κάποια bytes"
type: docs
weight: 30
url: /el/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

Λαμβάνει ή ορίζει τον αντιπρόσωπο που καλείται όταν έχουν εξαχθεί κάποια byte.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Παρατηρήσεις

Ο αποστολέας του συμβάντος είναι η παρουσία του [`ZstandardArchive`](../../zstandardarchive/) της οποίας η εξαγωγή προχωρά.

## Παραδείγματα

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


