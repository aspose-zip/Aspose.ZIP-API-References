---
title: "ArchiveLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Ιδιότητα ArchiveLoadOptions. Λαμβάνει ή ορίζει τον delegate που καλείται όταν έχουν εξαχθεί κάποια byte"
type: docs
weight: 50
url: /el/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Λαμβάνει ή ορίζει τον αντιπρόσωπο που καλείται όταν έχουν εξαχθεί κάποια byte.

```csharp
public EventHandler<ProgressCancelEventArgs> EntryExtractionProgressed { get; set; }
```

## Παρατηρήσεις

Ο αποστολέας του συμβάντος είναι η παρουσία του [`ArchiveEntry`](../../archiveentry/) της οποίας η εξαγωγή προχωρά.

## Παραδείγματα

Παρακολουθήστε την πρόοδο της εξαγωγής μιας καταχώρησης.

```csharp
var archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

Ακυρώστε την εξαγωγή μιας καταχώρησης μετά από κάποιο χρονικό διάστημα.

```csharp
Stopwatch watch = Stopwatch.StartNew();
using (Archive a = new Archive("big.zip", new ArchiveLoadOptions() {
    EntryExtractionProgressed = (s, e) => { if (watch.ElapsedMilliseconds > 1000) e.Cancel = true; } }))
{
    a.Entries[0].Extract("first.bin");
}
```

### Δείτε επίσης

* class [ProgressCancelEventArgs](../../progresscanceleventargs/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


