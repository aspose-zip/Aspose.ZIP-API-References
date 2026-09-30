---
title: "Κλάση GzipArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κλάση Aspose.Zip.Gzip.GzipArchive. Αυτή η κλάση αντιπροσωπεύει ένα αρχείο gzip. Χρησιμοποιήστε την για τη δημιουργία ή την εξαγωγή αρχείων gzip."
type: docs
weight: 510
url: /el/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο gzip. Χρησιμοποιήστε την για τη δημιουργία ή την εξαγωγή αρχείων gzip.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `GzipArchive` προετοιμασμένο για συμπίεση. |
| [GzipArchive](gziparchive/#constructor_2)(Stream, bool) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `GzipArchive` προετοιμασμένο για αποσυμπίεση. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, GzipLoadOptions) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `GzipArchive` προετοιμασμένο για αποσυμπίεση. |
| [GzipArchive](gziparchive/#constructor_4)(string, bool) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `GzipArchive` προετοιμασμένο για αποσυμπίεση. |
| [GzipArchive](gziparchive/#constructor_3)(string, GzipLoadOptions) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `GzipArchive` προετοιμασμένο για αποσυμπίεση. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | Όνομα του αρχικού αρχείου. |
| [UncompressedSize](../../aspose.zip.gzip/gziparchive/uncompressedsize/) { get; } | Λαμβάνει το μέγεθος ενός αρχικού αρχείου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | Εκτελεί εργασίες ορισμένες από την εφαρμογή που σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/#extract_1)(Stream) | Εξάγει το αρχείο στο παρεχόμενο ρεύμα. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/#extract)(string) | Εξάγει το αρχείο στο αρχείο με βάση τη διαδρομή. |
| [ExtractToDirectory](../../aspose.zip.gzip/gziparchive/extracttodirectory/)(string) | Εξάγει το περιεχόμενο του αρχείου στον παρεχόμενο φάκελο. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με το περιεχόμενο του αρχείου. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | Αποθηκεύει την αρχειοθήκη στο παρεχόμενο αρχείο προορισμού |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |

## Παρατηρήσεις

Ο αλγόριθμος συμπίεσης Gzip βασίζεται στον αλγόριθμο DEFLATE, ο οποίος είναι ένας συνδυασμός των LZ77 και Huffman κωδικοποίησης.

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* assembly [Aspose.Zip](../../)


