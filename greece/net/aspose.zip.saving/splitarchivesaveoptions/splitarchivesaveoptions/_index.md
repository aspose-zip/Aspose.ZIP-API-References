---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Aspose.ZIP για Αναφορά API .NET
description: SplitArchiveSaveOptions κατασκευαστής. Δημιουργεί τις ρυθμίσεις για την αποθήκευση ενός αρχείου zip πολλών τόμων.
type: docs
weight: 10
url: /el/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

Δημιουργεί τις ρυθμίσεις για την αποθήκευση ενός αρχείου zip πολλών τόμων.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Όνομα για τόμους. Μπορεί να είναι με ή χωρίς επέκταση .zip. |
| segmentSize | UInt32 | Μέγεθος όγκου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentOutOfRangeException | Το μέγεθος του τμήματος είναι μικρότερο από 65536 byte. |

### Παρατηρήσεις

Ορισμένοι τόμοι μπορεί να είναι μικρότεροι από*segmentSize*. Στις περισσότερες περιπτώσεις το τελευταίο τμήμα θα είναι μικρότερο, αλλά σπάνια μπορεί να είναι και τα κανονικά τμήματα.

Τα ονόματα των αρχείων θα είναι τα εξής:*fileName* .z01,*fileName* .z02, ...,*fileName* .z(n-1),*fileName*.φερμουάρ.

### Δείτε επίσης

* class [SplitArchiveSaveOptions](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* συνέλευση [Aspose.Zip](../../../)


