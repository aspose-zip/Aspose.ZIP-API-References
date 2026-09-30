---
title: "Κλάση TarArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.Tar.TarArchive class. Αυτή η κλάση αντιπροσωπεύει ένα αρχείο tar. Χρησιμοποιήστε την για να δημιουργήσετε, εξάγετε ή ενημερώσετε αρχεία tar."
type: docs
weight: 1270
url: /el/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο tar. Χρησιμοποιήστε την για τη δημιουργία, την εξαγωγή ή την ενημέρωση αρχείων tar.

```csharp
public class TarArchive : IArchive
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `TarArchive`. |
| [TarArchive](tararchive/#constructor_1)(Stream, TarLoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης `TarArchive` και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [TarArchive](tararchive/#constructor_2)(string, TarLoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης `TarArchive` και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | Λαμβάνει καταχωρήσεις τύπου [`TarEntry`](../tarentry/) που αποτελούν το αρχείο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | Εξάγει το παρεχόμενο gzip αρχείο και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | Εξάγει το παρεχόμενο gzip αρχείο και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromLZ4](../../aspose.zip.tar/tararchive/fromlz4/#fromlz4)(Stream) | Εξάγει το παρεχόμενο LZ4 αρχείο και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromLZ4](../../aspose.zip.tar/tararchive/fromlz4/#fromlz4_1)(string) | Εξάγει το παρεχόμενο LZ4 αρχείο και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | Εξάγει το παρεχόμενο lzip αρχείο και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | Εξάγει το παρεχόμενο lzip αρχείο και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromLZMA](../../aspose.zip.tar/tararchive/fromlzma/#fromlzma)(Stream) | Εξάγει το παρεχόμενο LZMA αρχείο και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromLZMA](../../aspose.zip.tar/tararchive/fromlzma/#fromlzma_1)(string) | Εξάγει το παρεχόμενο LZMA αρχείο και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | Εξάγει το παρεχόμενο αρχείο μορφής xz και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | Εξάγει το παρεχόμενο αρχείο μορφής xz και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | Εξάγει το παρεχόμενο αρχείο μορφής Z και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | Εξάγει το παρεχόμενο αρχείο μορφής Z και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromZstandard](../../aspose.zip.tar/tararchive/fromzstandard/#fromzstandard)(Stream) | Εξάγει το παρεχόμενο Zstandard αρχείο και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| static [FromZstandard](../../aspose.zip.tar/tararchive/fromzstandard/#fromzstandard_1)(string) | Εξάγει το παρεχόμενο Zstandard αρχείο και δημιουργεί ένα `TarArchive` από τα εξαγόμενα δεδομένα. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά από τον δοσμένο κατάλογο. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά από τον δοσμένο κατάλογο. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | Αφαιρεί την καταχώρηση από τη λίστα καταχωρίσεων με βάση το δείκτη. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | Εκτελεί εργασίες ορισμένες από την εφαρμογή που σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | Εξάγει όλα τα αρχεία στην αρχειοθήκη στον παρεχόμενο κατάλογο. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | Αποθηκεύει το αρχείο σε προορισμένο αρχείο που παρέχεται. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | Αποθηκεύει το αρχείο στο αρχείο μέσω διαδρομής με συμπίεση gzip. |
| [SaveLZ4Compressed](../../aspose.zip.tar/tararchive/savelz4compressed/#savelz4compressed)(Stream, TarFormat?) | Αποθηκεύει το αρχείο στη ροή με συμπίεση LZ4. |
| [SaveLZ4Compressed](../../aspose.zip.tar/tararchive/savelz4compressed/#savelz4compressed_1)(string, TarFormat?) | Αποθηκεύει το αρχείο στο αρχείο μέσω διαδρομής με συμπίεση LZ4. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | Αποθηκεύει το αρχείο στη ροή με συμπίεση lzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | Αποθηκεύει το αρχείο στο αρχείο μέσω διαδρομής με συμπίεση lzip. |
| [SaveLZMACompressed](../../aspose.zip.tar/tararchive/savelzmacompressed/#savelzmacompressed)(Stream, TarFormat?) | Αποθηκεύει το αρχείο στη ροή με συμπίεση LZMA. |
| [SaveLZMACompressed](../../aspose.zip.tar/tararchive/savelzmacompressed/#savelzmacompressed_1)(string, TarFormat?) | Αποθηκεύει το αρχείο στο αρχείο μέσω διαδρομής με συμπίεση lzma. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Αποθηκεύει το αρχείο στη ροή με συμπίεση xz. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Αποθηκεύει το αρχείο στη διαδρομή μέσω διαδρομής με συμπίεση xz. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Αποθηκεύει το αρχείο στη ροή με συμπίεση Z. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Αποθηκεύει το αρχείο στη διαδρομή μέσω διαδρομής με συμπίεση Z. |
| [SaveZstandard](../../aspose.zip.tar/tararchive/savezstandard/#savezstandard)(Stream, TarFormat?) | Αποθηκεύει το αρχείο στο ρεύμα με συμπίεση Zstandard. |
| [SaveZstandard](../../aspose.zip.tar/tararchive/savezstandard/#savezstandard_1)(string, TarFormat?) | Αποθηκεύει το αρχείο στο αρχείο μέσω διαδρομής με συμπίεση Zstandard. |

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Tar](../../aspose.zip.tar/)
* assembly [Aspose.Zip](../../)


