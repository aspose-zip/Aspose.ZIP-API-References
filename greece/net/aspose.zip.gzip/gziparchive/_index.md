---
title: Class GzipArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: Aspose.Zip.Gzip.GzipArchive τάξη. Αυτή η κλάση αντιπροσωπεύει το αρχείο αρχειοθέτησης gzip. Χρησιμοποιήστε το για να συνθέσετε ή να εξαγάγετε αρχεία gzip.
type: docs
weight: 210
url: /el/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

Αυτή η κλάση αντιπροσωπεύει το αρχείο αρχειοθέτησης gzip. Χρησιμοποιήστε το για να συνθέσετε ή να εξαγάγετε αρχεία gzip.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | Αρχικοποιεί μια νέα παρουσία του`GzipArchive` τάξη προετοιμασμένη για συμπίεση. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | Αρχικοποιεί μια νέα παρουσία του`GzipArchive` τάξη προετοιμασμένη για αποσυμπίεση. |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | Αρχικοποιεί μια νέα παρουσία του`GzipArchive` τάξη. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | Όνομα αρχικού αρχείου. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | Εκτελεί εργασίες που καθορίζονται από την εφαρμογή που σχετίζονται με την απελευθέρωση, την απελευθέρωση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | Εξάγει το αρχείο στη ροή που παρέχεται. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με περιεχόμενο αρχειοθέτησης. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | Αποθηκεύει το αρχείο στη ροή που παρέχεται. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | Αποθηκεύει το αρχείο στο παρεχόμενο αρχείο προορισμού. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου. |

### Παρατηρήσεις

Ο αλγόριθμος συμπίεσης Gzip βασίζεται στον αλγόριθμο DEFLATE, ο οποίος είναι ένας συνδυασμός κωδικοποίησης LZ77 και Huffman.

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* χώρος ονομάτων [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* συνέλευση [Aspose.Zip](../../)


