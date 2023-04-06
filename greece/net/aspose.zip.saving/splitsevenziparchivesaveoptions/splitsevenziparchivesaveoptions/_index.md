---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Aspose.ZIP για Αναφορά API .NET
description: SplitSevenZipArchiveSaveOptions κατασκευαστής. Δημιουργεί τις ρυθμίσεις για την αποθήκευση ενός αρχείου πολλών τόμων 7z.
type: docs
weight: 10
url: /el/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Δημιουργεί τις ρυθμίσεις για την αποθήκευση ενός αρχείου πολλών τόμων 7z.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Όνομα για τόμους. Μπορεί να είναι με ή χωρίς επέκταση .7z. |
| segmentSize | UInt32 | Μέγεθος όγκου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* είναι λιγότερο από 100. |

### Παρατηρήσεις

Ορισμένοι τόμοι μπορεί να είναι μικρότεροι από*segmentSize*. Στις περισσότερες περιπτώσεις το τελευταίο τμήμα θα είναι μικρότερο, αλλά σπάνια μπορεί να είναι και τα κανονικά τμήματα.

Τα ονόματα των αρχείων θα είναι τα εξής:*fileName* .7z.001,*fileName* .7z.002, ...,*fileName*.7z.(n).

### Δείτε επίσης

* class [SplitSevenZipArchiveSaveOptions](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* συνέλευση [Aspose.Zip](../../../)


