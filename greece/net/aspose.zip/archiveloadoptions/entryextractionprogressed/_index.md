---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP για Αναφορά API .NET
description: ArchiveLoadOptions ιδιοκτησία. Λαμβάνει ή ορίζει τον εκπρόσωπο που καλείται όταν έχουν εξαχθεί ορισμένα byte.
type: docs
weight: 40
url: /el/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Λαμβάνει ή ορίζει τον εκπρόσωπο που καλείται όταν έχουν εξαχθεί ορισμένα byte.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### Παρατηρήσεις

Ο αποστολέας του συμβάντος είναι ο[`ArchiveEntry`](../../archiveentry/) περίπτωση στην οποία προχωρά η εξαγωγή.

### Παραδείγματα

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### Δείτε επίσης

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* χώρος ονομάτων [Aspose.Zip](../../archiveloadoptions/)
* συνέλευση [Aspose.Zip](../../../)


