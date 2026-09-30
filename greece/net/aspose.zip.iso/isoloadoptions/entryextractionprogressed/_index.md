---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Ιδιότητα IsoLoadOptions. Λαμβάνει ή ορίζει τον αντιπρόσωπο που καλείται όταν έχουν εξαχθεί κάποια bytes"
type: docs
weight: 30
url: /el/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

Λαμβάνει ή ορίζει τον αντιπρόσωπο που καλείται όταν έχουν εξαχθεί κάποια byte.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Παρατηρήσεις

Ο αποστολέας του γεγονότος είναι το παράδειγμα [`IsoEntry`](../../isoentry/) του οποίου η εξαγωγή προχωρά.

## Παραδείγματα

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


