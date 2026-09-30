---
title: "Κλάση RarArchiveEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.Rar.RarArchiveEntry κλάση. Αντιπροσωπεύει ένα μεμονωμένο αρχείο μέσα στο αρχείο."
type: docs
weight: 800
url: /el/net/aspose.zip.rar/rararchiveentry/
---
## RarArchiveEntry class

Αναπαριστά ένα μοναδικό αρχείο μέσα σε ένα αρχείο.

```csharp
public abstract class RarArchiveEntry : IArchiveFileEntry
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | Λαμβάνει το μέγεθος ενός συμπιεσμένου αρχείου. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | Λαμβάνει την ημερομηνία και ώρα δημιουργίας. |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | Επιστρέφει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο. |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | Λαμβάνει την ημερομηνία και ώρα τελευταίας πρόσβασης. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | Λαμβάνει την ημερομηνία και ώρα τελευταίας τροποποίησης. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | Επιστρέφει το όνομα της καταχώρησης μέσα στο αρχείο. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | Λαμβάνει το μέγεθος ενός αρχικού αρχείου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract_1)(Stream, string) | Εξάγει την καταχώρηση στη δοθείσα ροή. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract)(string, string) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη δοθείσα διαδρομή. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το αποσυμπιεσμένο περιεχόμενο της καταχώρησης. |

## Συμβάντα

| Όνομα | Περιγραφή |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής εξάγεται. |

## Παρατηρήσεις

Μετατρέψτε μια παρουσία `RarArchiveEntry` σε [`RarArchiveEntryEncrypted`](../rararchiveentryencrypted/) για να προσδιορίσετε εάν η καταχώρηση είναι κρυπτογραφημένη ή όχι.

### Δείτε επίσης

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Rar](../../aspose.zip.rar/)
* assembly [Aspose.Zip](../../)


