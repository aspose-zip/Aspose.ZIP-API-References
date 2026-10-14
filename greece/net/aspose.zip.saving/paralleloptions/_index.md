---
title: "Κλάση ParallelOptions"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.Saving.ParallelOptions class. Επιλογές για παράλληλη συμπίεση"
type: docs
weight: 990
url: /el/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

Επιλογές για παράλληλη συμπίεση.

```csharp
public class ParallelOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | Αποκτά ή ορίζει εκτίμηση μνήμης σε megabytes διαθέσιμη για να φιλοξενήσει συμπιεσμένες καταχωρήσεις χωρίς ανταλλαγή σε δίσκο. Αυτή η τιμή έχει νόημα μόνο εάν η ρύθμιση [`ParallelCompressInMemory`](./parallelcompressinmemory/) είναι σε λειτουργία Auto. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | Αποκτά ή ορίζει τιμή που υποδεικνύει πώς θα χρησιμοποιηθεί η παράλληλη προσέγγιση. |

## Παρατηρήσεις

Αυτές οι επιλογές διαχειρίζονται τη συγχρονισμένη συμπίεση από πολλούς πυρήνες CPU.

## Παραδείγματα

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = ParallelCompressionMode.Auto, AvailableMemorySize = 4000 } });
}
```

### Δείτε επίσης

* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


