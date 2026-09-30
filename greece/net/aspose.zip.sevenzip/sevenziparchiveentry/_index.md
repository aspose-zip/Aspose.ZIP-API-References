---
title: "Κλάση SevenZipArchiveEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.SevenZip.SevenZipArchiveEntry κλάση. Αντιπροσωπεύει ένα μεμονωμένο αρχείο μέσα σε αρχείο 7z"
type: docs
weight: 1200
url: /el/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

Αντιπροσωπεύει ένα μεμονωμένο αρχείο μέσα σε ένα αρχείο 7z.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Λαμβάνει το μέγεθος ενός συμπιεσμένου αρχείου. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Επιστρέφει τις ρυθμίσεις για συμπίεση ή αποσυμπίεση. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Επιστρέφει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Λαμβάνει την ημερομηνία και ώρα τελευταίας τροποποίησης. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Επιστρέφει το όνομα της καταχώρησης μέσα στο αρχείο. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Λαμβάνει το μέγεθος ενός αρχικού αρχείου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | Εξάγει την καταχώρηση στη δοθείσα ροή. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη δοθείσα διαδρομή. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει ένα ρεύμα με το περιεχόμενο της καταχώρησης. |

## Συμβάντα

| Όνομα | Περιγραφή |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής συμπιέζεται. |

## Παρατηρήσεις

Μετατρέψτε μια παρουσία του `SevenZipArchiveEntry` σε [`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) για να προσδιορίσετε εάν η καταχώρηση είναι κρυπτογραφημένη ή όχι.

### Δείτε επίσης

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assembly [Aspose.Zip](../../)


