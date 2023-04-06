---
title: Class ParallelOptions
second_title: Aspose.ZIP για Αναφορά API .NET
description: Aspose.Zip.Saving.ParallelOptions τάξη. Επιλογές για παράλληλη συμπίεση.
type: docs
weight: 490
url: /el/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

Επιλογές για παράλληλη συμπίεση.

```csharp
public class ParallelOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | Λαμβάνει ή ορίζει εκτίμηση μνήμης σε megabyte διαθέσιμα για την υποδοχή συμπιεσμένων καταχωρήσεων χωρίς εναλλαγή στο δίσκο. Αυτή η τιμή έχει νόημα μόνο εάν[`ParallelCompressInMemory`](./parallelcompressinmemory/) η ρύθμιση είναι μέσαAuto mode. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | Λαμβάνει ή ορίζει τιμή που υποδεικνύει πώς θα χρησιμοποιηθεί η παράλληλη προσέγγιση. |

### Παρατηρήσεις

Αυτές οι επιλογές διαχειρίζονται την ταυτόχρονη συμπίεση από πολλούς πυρήνες CPU.

### Παραδείγματα

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = mode, AvailableMemorySize = 4000 } });
}
```

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Zip.Saving](../../aspose.zip.saving/)
* συνέλευση [Aspose.Zip](../../)


