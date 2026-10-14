---
title: "SplitArchiveSaveOptions.SplitArchiveSaveOptions"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής SplitArchiveSaveOptions. Δημιουργεί τις ρυθμίσεις για την αποθήκευση ενός πολυτόμου αρχείου ZIP."
type: docs
weight: 10
url: /el/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions(string, uint) {#constructor}

Δημιουργεί στιγμιότυπα ρυθμίσεων για την αποθήκευση ενός πολυτόμου αρχείου ZIP.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Όνομα για τους τόμους. Μπορεί να είναι με ή χωρίς την επέκταση .zip. |
| segmentSize | UInt32 | Μέγεθος ενός τόμου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | Το μέγεθος του τμήματος είναι μικρότερο από 65536 bytes. |

## Παρατηρήσεις

Ορισμένοι τόμοι μπορεί να είναι μικρότεροι από το *segmentSize*. Στις περισσότερες περιπτώσεις, το τελευταίο τμήμα θα είναι μικρότερο, αλλά σπάνια τα κανονικά τμήματα μπορεί να είναι επίσης.

Τα ονόματα των αρχείων θα είναι ως εξής: *fileName*.z01, *fileName*.z02, ..., *fileName*.z(n-1), *fileName*.zip.

### Δείτε επίσης

* class [SplitArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)

---

## SplitArchiveSaveOptions(uint) {#constructor_1}

Δημιουργεί στιγμιότυπα ρυθμίσεων για την αποθήκευση ενός πολυτόμου αρχείου ZIP.

```csharp
public SplitArchiveSaveOptions(uint segmentSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| segmentSize | UInt32 | Μέγεθος ενός τόμου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | Το μέγεθος του τμήματος είναι μικρότερο από 65536 bytes. |

## Παρατηρήσεις

Χρησιμοποιήστε αυτήν την παρουσία `SplitArchiveSaveOptions` χωρίς όνομα αρχείου με τη μέθοδο [`SaveSplit`](../../../aspose.zip/archive/savesplit/).

Ορισμένοι τόμοι μπορεί να είναι μικρότεροι από το *segmentSize*. Στις περισσότερες περιπτώσεις, το τελευταίο τμήμα θα είναι μικρότερο, αλλά σπάνια τα κανονικά τμήματα μπορεί να είναι επίσης.

### Δείτε επίσης

* class [SplitArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


