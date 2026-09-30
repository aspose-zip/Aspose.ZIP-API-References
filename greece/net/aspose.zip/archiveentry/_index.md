---
title: "Κλάση ArchiveEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κλάση Aspose.Zip.ArchiveEntry. Αντιπροσωπεύει ένα μεμονωμένο αρχείο μέσα σε ένα αρχείο."
type: docs
weight: 170
url: /el/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

Αναπαριστά ένα μοναδικό αρχείο μέσα σε ένα αρχείο.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Επιστρέφει το σχόλιο της καταχώρησης μέσα στο αρχείο. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Επιστρέφει το μέγεθος του συμπιεσμένου αρχείου. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Επιστρέφει τις ρυθμίσεις για συμπίεση ή αποσυμπίεση. |
| [DataSource](../../aspose.zip/archiveentry/datasource/) { get; } | Πηγή για την καταχώρηση εάν η καταχώρηση προστέθηκε στο αρχείο, χωρίς εξαγωγή. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Επιστρέφει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία και ώρα τελευταίας τροποποίησης. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Επιστρέφει το όνομα της καταχώρησης μέσα στο αρχείο. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Επιστρέφει το μέγεθος του αρχικού αρχείου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | Εξάγει την καταχώρηση στη δοθείσα ροή. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη δοθείσα διαδρομή. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το αποσυμπιεσμένο περιεχόμενο της καταχώρησης. |

## Συμβάντα

| Όνομα | Περιγραφή |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής συμπιέζεται. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής εξάγεται. |

## Παρατηρήσεις

Μετατρέψτε μια παρουσία `ArchiveEntry` σε [`ArchiveEntryEncrypted`](../archiveentryencrypted/) για να προσδιορίσετε εάν η καταχώρηση είναι κρυπτογραφημένη ή όχι.

### Δείτε επίσης

* interface [IArchiveFileEntry](../iarchivefileentry/)
* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


