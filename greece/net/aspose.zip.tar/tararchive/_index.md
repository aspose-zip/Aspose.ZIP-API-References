---
title: Class TarArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: Aspose.Zip.Tar.TarArchive τάξη. Αυτή η κλάση αντιπροσωπεύει το αρχείο αρχειοθέτησης tar. Χρησιμοποιήστε το για να συνθέσετε να εξαγάγετε ή να ενημερώσετε αρχεία tar.
type: docs
weight: 730
url: /el/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Αυτή η κλάση αντιπροσωπεύει το αρχείο αρχειοθέτησης tar. Χρησιμοποιήστε το για να συνθέσετε, να εξαγάγετε ή να ενημερώσετε αρχεία tar.

```csharp
public class TarArchive : IArchive
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | Αρχικοποιεί μια νέα παρουσία του`TarArchive` τάξη. |
| [TarArchive](tararchive/#constructor_1)(Stream) | Αρχικοποιεί μια νέα παρουσία του[`Archive`](../../aspose.zip/archive/) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο. |
| [TarArchive](tararchive/#constructor_2)(string) | Αρχικοποιεί μια νέα παρουσία του`TarArchive` Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | Λαμβάνει καταχωρήσεις του[`TarEntry`](../tarentry/) τύπος που αποτελεί το αρχείο. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | Εξάγει το παρεχόμενο αρχείο gzip και συνθέτει`TarArchive` από εξαγόμενα δεδομένα. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | Εξάγει το παρεχόμενο αρχείο gzip και συνθέτει`TarArchive` από εξαγόμενα δεδομένα. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | Εξάγει το παρεχόμενο αρχείο lzip και συνθέτει`TarArchive` από εξαγόμενα δεδομένα. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | Εξάγει το παρεχόμενο αρχείο lzip και συνθέτει`TarArchive` από εξαγόμενα δεδομένα. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | Εξάγει το παρεχόμενο αρχείο μορφής xz και συνθέτει`TarArchive` από εξαγόμενα δεδομένα. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | Εξάγει το παρεχόμενο αρχείο μορφής xz και συνθέτει`TarArchive` από εξαγόμενα δεδομένα. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | Εξάγει το παρεχόμενο αρχείο μορφής Z και συνθέτει`TarArchive` από εξαγόμενα δεδομένα. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | Εξάγει το παρεχόμενο αρχείο μορφής Z και συνθέτει`TarArchive` από εξαγόμενα δεδομένα. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | Αφαιρεί την καταχώρηση από τη λίστα καταχωρήσεων κατά ευρετήριο. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | Καταργεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρισης από τη λίστα καταχωρήσεων. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | Εκτελεί εργασίες που καθορίζονται από την εφαρμογή που σχετίζονται με την απελευθέρωση, την απελευθέρωση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | Εξάγει όλα τα αρχεία στο αρχείο στον παρεχόμενο κατάλογο. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | Αποθηκεύει το αρχείο στη ροή που παρέχεται. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | Αποθηκεύει το αρχείο στο παρεχόμενο αρχείο προορισμού. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | Αποθηκεύει το αρχείο στο αρχείο κατά διαδρομή με συμπίεση gzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | Αποθηκεύει το αρχείο στη ροή με συμπίεση lzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | Αποθηκεύει το αρχείο στο αρχείο κατά διαδρομή με συμπίεση lzip. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Αποθηκεύει το αρχείο στη ροή με συμπίεση xz. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Αποθηκεύει το αρχείο στη διαδρομή ανά διαδρομή με συμπίεση xz. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Αποθηκεύει το αρχείο στη ροή με συμπίεση Z. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Αποθηκεύει το αρχείο στη διαδρομή ανά διαδρομή με συμπίεση Z. |

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* χώρος ονομάτων [Aspose.Zip.Tar](../../aspose.zip.tar/)
* συνέλευση [Aspose.Zip](../../)


