---
title: "SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής SplitSevenZipArchiveSaveOptions. Δημιουργεί ρυθμίσεις για την αποθήκευση ενός πολυτόμου αρχείου 7z"
type: docs
weight: 10
url: /el/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Δημιουργεί τις ρυθμίσεις για την αποθήκευση ενός πολυτόμου αρχείου 7z.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Όνομα για τους τόμους. Μπορεί να είναι με ή χωρίς την επέκταση .7z. |
| segmentSize | UInt32 | Μέγεθος του τόμου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* είναι μικρότερο από 100. |

## Παρατηρήσεις

Ορισμένοι τόμοι μπορεί να είναι μικρότεροι από το *segmentSize*. Στις περισσότερες περιπτώσεις, το τελευταίο τμήμα θα είναι μικρότερο, αλλά σπάνια τα κανονικά τμήματα μπορεί να είναι επίσης.

Τα ονόματα των αρχείων θα είναι ως εξής: *fileName*.7z.001, *fileName*.7z.002, ..., *fileName*.7z.(n).

### Δείτε επίσης

* class [SplitSevenZipArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


