---
title: Class ArchiveEntry
second_title: Aspose.ZIP για Αναφορά API .NET
description: Aspose.Zip.ArchiveEntry τάξη. Αντιπροσωπεύει μεμονωμένο αρχείο μέσα στο αρχείο.
type: docs
weight: 20
url: /el/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

Αντιπροσωπεύει μεμονωμένο αρχείο μέσα στο αρχείο.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Λαμβάνει σχόλιο για την καταχώρηση μέσα στο αρχείο. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Παίρνει το μέγεθος του συμπιεσμένου αρχείου. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Λαμβάνει ρυθμίσεις για συμπίεση ή αποσυμπίεση. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει τον κατάλογο. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία και την ώρα της τελευταίας τροποποίησης. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Λαμβάνει το όνομα της καταχώρησης μέσα στο αρχείο. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Παίρνει το μέγεθος του αρχικού αρχείου. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | Εξάγει την καταχώρηση στο σύστημα αρχείων από τη διαδρομή που παρέχεται. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με αποσυμπιεσμένο περιεχόμενο καταχώρισης. |

## Εκδηλώσεις

| Ονομα | Περιγραφή |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Αυξάνεται όταν συμπιέζεται ένα τμήμα της ακατέργαστης ροής. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Αυξάνεται όταν εξάγεται ένα τμήμα της ακατέργαστης ροής. |

### Παρατηρήσεις

Ρίξτε μια`ArchiveEntry` παράδειγμα προς[`ArchiveEntryEncrypted`](../archiveentryencrypted/) για να προσδιορίσετε εάν η καταχώρηση είναι κρυπτογραφημένη ή όχι.

### Δείτε επίσης

* interface [IArchiveFileEntry](../iarchivefileentry/)
* χώρος ονομάτων [Aspose.Zip](../../aspose.zip/)
* συνέλευση [Aspose.Zip](../../)


