---
title: Class SevenZipArchiveEntry
second_title: Aspose.ZIP για Αναφορά API .NET
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry τάξη. Αντιπροσωπεύει μεμονωμένο αρχείο εντός αρχείου 7z.
type: docs
weight: 670
url: /el/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

Αντιπροσωπεύει μεμονωμένο αρχείο εντός αρχείου 7z.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Παίρνει το μέγεθος του συμπιεσμένου αρχείου. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Λαμβάνει ρυθμίσεις για συμπίεση ή αποσυμπίεση. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει τον κατάλογο. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Λαμβάνει ημερομηνία και ώρα τελευταίας τροποποίησης. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Λαμβάνει το όνομα της καταχώρησης μέσα στο αρχείο. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Παίρνει το μέγεθος του αρχικού αρχείου. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | Εξάγει την καταχώρηση στο σύστημα αρχείων από τη διαδρομή που παρέχεται. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με περιεχόμενο καταχώρισης. |

## Εκδηλώσεις

| Ονομα | Περιγραφή |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Αυξάνεται όταν συμπιέζεται ένα τμήμα της ακατέργαστης ροής. |

### Παρατηρήσεις

Ρίξτε μια`SevenZipArchiveEntry` παράδειγμα προς[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) για να προσδιορίσετε εάν η καταχώρηση είναι κρυπτογραφημένη ή όχι.

### Δείτε επίσης

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* συνέλευση [Aspose.Zip](../../)


