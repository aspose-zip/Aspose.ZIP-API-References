---
title: "Κλάση AlzEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.Alz.AlzEntry κλάση. Αντιπροσωπεύει μια καταχώρηση αρχείου σε ένα αρχείο ALZ με όλα τα μεταδεδομένα του"
type: docs
weight: 30
url: /el/net/aspose.zip.alz/alzentry/
---
## AlzEntry class

Αντιπροσωπεύει μια καταχώρηση αρχείου σε μια αρχειοθήκη ALZ με όλα τα μεταδεδομένα της.

```csharp
public abstract class AlzEntry : IArchiveFileEntry
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | Συμπιεσμένο μέγεθος των δεδομένων του αρχείου σε bytes. |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | Επιστρέφει true εάν αυτή η καταχώρηση αντιπροσωπεύει έναν φάκελο. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | Όνομα αρχείου (χωρίς διαδρομή). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | Μη συμπιεσμένο μέγεθος των δεδομένων του αρχείου σε byte. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract_1)(Stream, string) | Εξάγει την καταχώρηση στη δοθείσα ροή. |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract)(string, string) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη δοθείσα διαδρομή. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το αποσυμπιεσμένο περιεχόμενο της καταχώρησης. |

### Δείτε επίσης

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


