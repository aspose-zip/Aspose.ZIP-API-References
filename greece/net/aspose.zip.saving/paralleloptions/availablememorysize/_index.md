---
title: ParallelOptions.AvailableMemorySize
second_title: Aspose.ZIP για Αναφορά API .NET
description: ParallelOptions ιδιοκτησία. Λαμβάνει ή ορίζει εκτίμηση μνήμης σε megabyte διαθέσιμα για την υποδοχή συμπιεσμένων καταχωρήσεων χωρίς εναλλαγή στο δίσκο. Αυτή η τιμή έχει νόημα μόνο εάνParallelCompressInMemory η ρύθμιση είναι μέσαAuto mode.
type: docs
weight: 20
url: /el/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

Λαμβάνει ή ορίζει εκτίμηση μνήμης σε megabyte διαθέσιμα για την υποδοχή συμπιεσμένων καταχωρήσεων χωρίς εναλλαγή στο δίσκο. Αυτή η τιμή έχει νόημα μόνο εάν[`ParallelCompressInMemory`](../parallelcompressinmemory/) η ρύθμιση είναι μέσαAuto mode.

```csharp
public int AvailableMemorySize { get; set; }
```

### Παρατηρήσεις

Αυτή η τιμή χρησιμοποιείται για τον υπολογισμό του μεγαλύτερου μεγέθους καταχώρισης που μπορεί να συμπιεστεί παράλληλα με άλλες. Όλες οι εγγραφές πάνω από το υπολογιζόμενο όριο θα συμπιεστούν διαδοχικά. Είναι ασφαλές να έχετε`AvailableMemorySize` ιδιοκτησία τόσο μεγάλη όσο η δωρεάν μνήμη RAM και ακόμη μεγαλύτερη. Από προεπιλογή, υποτίθεται ότι έχετε τουλάχιστον 200 MB ανά πυρήνα CPU.

### Δείτε επίσης

* class [ParallelOptions](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../paralleloptions/)
* συνέλευση [Aspose.Zip](../../../)


