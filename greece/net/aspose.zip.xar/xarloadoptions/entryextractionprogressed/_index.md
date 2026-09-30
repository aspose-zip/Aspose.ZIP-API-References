---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Ιδιότητα XarLoadOptions. Λαμβάνει ή ορίζει τον αντιπρόσωπο που καλείται όταν έχουν εξαχθεί κάποια bytes"
type: docs
weight: 30
url: /el/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

Λαμβάνει ή ορίζει τον αντιπρόσωπο που καλείται όταν έχουν εξαχθεί κάποια byte.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Παρατηρήσεις

Ο αποστολέας του συμβάντος είναι το αντικείμενο [`XarFileEntry`](../../xarfileentry/) του οποίου η εξαγωγή προχωρά.

## Παραδείγματα

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### Δείτε επίσης

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


