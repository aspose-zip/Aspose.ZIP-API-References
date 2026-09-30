---
title: "Κλάση Bzip2Archive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.Bzip2.Bzip2Archive κλάση. Αυτή η κλάση αντιπροσωπεύει ένα αρχείο bzip2. Χρησιμοποιήστε την για τη σύνθεση ή την εξαγωγή αρχείων bzip2."
type: docs
weight: 280
url: /el/net/aspose.zip.bzip2/bzip2archive/
---
## Bzip2Archive class

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο bzip2. Χρησιμοποιήστε την για τη δημιουργία ή την εξαγωγή αρχείων bzip2.

```csharp
public class Bzip2Archive : IArchive, IArchiveFileEntry
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Bzip2Archive](bzip2archive/#constructor)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `Bzip2Archive` προετοιμασμένο για συμπίεση. |
| [Bzip2Archive](bzip2archive/#constructor_1)(Stream, Bzip2LoadOptions) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `Bzip2Archive` προετοιμασμένο για αποσυμπίεση. |
| [Bzip2Archive](bzip2archive/#constructor_2)(string, Bzip2LoadOptions) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `Bzip2Archive` προετοιμασμένο για αποσυμπίεση. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Dispose](../../aspose.zip.bzip2/bzip2archive/dispose/)() | Εκτελεί εργασίες ορισμένες από την εφαρμογή που σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/#extract_1)(Stream) | Εξάγει το αρχείο στο παρεχόμενο ρεύμα. |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/#extract)(string) | Εξάγει το αρχείο στο αρχείο με βάση τη διαδρομή. |
| [ExtractToDirectory](../../aspose.zip.bzip2/bzip2archive/extracttodirectory/)(string) | Εξάγει το περιεχόμενο του αρχείου στον παρεχόμενο φάκελο. |
| [Open](../../aspose.zip.bzip2/bzip2archive/open/)() | Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με το περιεχόμενο του αρχείου. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save)(Stream, Bzip2SaveOptions) | Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save_1)(string, Bzip2SaveOptions) | Αποθηκεύει το αρχείο σε προορισμένο αρχείο που παρέχεται. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_2)(FileInfo) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_3)(Stream) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_4)(string) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource)(CpioArchive, CpioFormat) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_1)(TarArchive, TarFormat) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |

## Παρατηρήσεις

Το bzip2 συμπιέζει αρχεία χρησιμοποιώντας τον αλγόριθμο συμπίεσης κειμένου με ταξινόμηση μπλοκ Burrows-Wheeler και την κωδικοποίηση Huffman. Δείτε περισσότερα: https://en.wikipedia.org/wiki/Bzip2

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Bzip2](../../aspose.zip.bzip2/)
* assembly [Aspose.Zip](../../)


