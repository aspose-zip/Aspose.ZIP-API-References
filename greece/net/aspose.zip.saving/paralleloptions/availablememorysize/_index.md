---
title: "ParallelOptions.AvailableMemorySize"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Ιδιότητα ParallelOptions. Λαμβάνει ή ορίζει εκτίμηση μνήμης σε megabytes που είναι διαθέσιμη για να φιλοξενήσει συμπιεσμένες καταχωρίσεις χωρίς εναλλαγή σε δίσκο. Αυτή η τιμή έχει νόημα μόνο εάν η ρύθμιση ParallelCompressInMemory είναι σε λειτουργία Auto"
type: docs
weight: 20
url: /el/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

Λαμβάνει ή ορίζει εκτίμηση μνήμης σε megabytes που είναι διαθέσιμη για να φιλοξενήσει συμπιεσμένες καταχωρίσεις χωρίς εναλλαγή σε δίσκο. Αυτή η τιμή έχει νόημα μόνο εάν η ρύθμιση [`ParallelCompressInMemory`](../parallelcompressinmemory/) είναι σε λειτουργία Auto.

```csharp
public int AvailableMemorySize { get; set; }
```

## Παρατηρήσεις

Αυτή η τιμή χρησιμοποιείται για τον υπολογισμό του μέγιστου μεγέθους μιας καταχώρισης που μπορεί να συμπιεστεί παράλληλα με άλλες. Όλες οι καταχωρίσεις πάνω από το υπολογισμένο όριο θα συμπιεστούν διαδοχικά. Είναι ασφαλές να έχετε την ιδιότητα `AvailableMemorySize` τόσο μεγάλη όσο η ελεύθερη RAM και ακόμη μεγαλύτερη. Από προεπιλογή, υποτίθεται ότι έχετε τουλάχιστον 200 MB ανά πυρήνα CPU.

### Δείτε επίσης

* class [ParallelOptions](../)
* namespace [Aspose.Zip.Saving](../../paralleloptions/)
* assembly [Aspose.Zip](../../../)


