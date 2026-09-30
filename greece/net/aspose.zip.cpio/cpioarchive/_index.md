---
title: "Κλάση CpioArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.Cpio.CpioArchive class. Αυτή η κλάση αντιπροσωπεύει αρχείο cpio"
type: docs
weight: 410
url: /el/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

Αυτή η κλάση αντιπροσωπεύει αρχείο cpio

```csharp
public class CpioArchive : IArchive
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `CpioArchive`. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | Αρχικοποιεί μια νέα παρουσία της κλάσης `CpioArchive` και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | Αρχικοποιεί μια νέα παρουσία της κλάσης `CpioArchive` και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | Λαμβάνει καταχωρήσεις τύπου [`CpioEntry`](../cpioentry/) που αποτελούν το αρχείο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά από τον δοσμένο κατάλογο. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά από τον δοσμένο κατάλογο. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | Αφαιρεί την καταχώρηση από τη λίστα καταχωρίσεων με βάση το δείκτη. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | Εκτελεί εργασίες ορισμένες από την εφαρμογή που σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | Εξάγει όλα τα αρχεία στην αρχειοθήκη στον παρεχόμενο κατάλογο. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | Αποθηκεύει το αρχείο σε προορισμένο αρχείο που παρέχεται. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | Αποθηκεύει το αρχείο στο αρχείο μέσω διαδρομής με συμπίεση gzip. |
| [SaveLzipped](../../aspose.zip.cpio/cpioarchive/savelzipped/#savelzipped)(Stream, CpioFormat) | Αποθηκεύει το αρχείο στη ροή με συμπίεση lzip. |
| [SaveLzipped](../../aspose.zip.cpio/cpioarchive/savelzipped/#savelzipped_1)(string, CpioFormat) | Αποθηκεύει το αρχείο στο αρχείο μέσω διαδρομής με συμπίεση lzip. |
| [SaveLZMACompressed](../../aspose.zip.cpio/cpioarchive/savelzmacompressed/#savelzmacompressed)(Stream, CpioFormat) | Αποθηκεύει το αρχείο στη ροή με συμπίεση LZMA. |
| [SaveLZMACompressed](../../aspose.zip.cpio/cpioarchive/savelzmacompressed/#savelzmacompressed_1)(string, CpioFormat) | Αποθηκεύει το αρχείο στο αρχείο μέσω διαδρομής με συμπίεση lzma. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | Αποθηκεύει το αρχείο στη ροή με συμπίεση xz. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | Αποθηκεύει το αρχείο στη διαδρομή μέσω διαδρομής με συμπίεση xz. |
| [SaveZCompressed](../../aspose.zip.cpio/cpioarchive/savezcompressed/#savezcompressed)(Stream, CpioFormat) | Αποθηκεύει το αρχείο στη ροή με συμπίεση Z. |
| [SaveZCompressed](../../aspose.zip.cpio/cpioarchive/savezcompressed/#savezcompressed_1)(string, CpioFormat) | Αποθηκεύει το αρχείο στη διαδρομή μέσω διαδρομής με συμπίεση Z. |
| [SaveZstandard](../../aspose.zip.cpio/cpioarchive/savezstandard/#savezstandard)(Stream, CpioFormat) | Αποθηκεύει το αρχείο στο ρεύμα με συμπίεση Zstandard. |
| [SaveZstandard](../../aspose.zip.cpio/cpioarchive/savezstandard/#savezstandard_1)(string, CpioFormat) | Αποθηκεύει το αρχείο στο αρχείο μέσω διαδρομής με συμπίεση Zstandard. |

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* assembly [Aspose.Zip](../../)


