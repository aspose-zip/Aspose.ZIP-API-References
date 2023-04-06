---
title: Class CpioArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: Aspose.Zip.Cpio.CpioArchive τάξη. Αυτή η κλάση αντιπροσωπεύει το αρχείο αρχειοθέτησης cpio.
type: docs
weight: 160
url: /el/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

Αυτή η κλάση αντιπροσωπεύει το αρχείο αρχειοθέτησης cpio.

```csharp
public class CpioArchive : IArchive
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | Αρχικοποιεί μια νέα παρουσία του`CpioArchive` τάξη. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | Αρχικοποιεί μια νέα παρουσία του`CpioArchive` Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | Αρχικοποιεί μια νέα παρουσία του`CpioArchive` Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | Λαμβάνει καταχωρήσεις του[`CpioEntry`](../cpioentry/) τύπος που αποτελεί το αρχείο. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | Καταργεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρισης από τη λίστα καταχωρήσεων. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | Αφαιρεί την καταχώρηση από τη λίστα καταχωρήσεων κατά ευρετήριο. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | Εκτελεί εργασίες που καθορίζονται από την εφαρμογή που σχετίζονται με την απελευθέρωση, την απελευθέρωση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | Εξάγει όλα τα αρχεία στο αρχείο στον παρεχόμενο κατάλογο. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | Αποθηκεύει το αρχείο στη ροή που παρέχεται. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | Αποθηκεύει το αρχείο στο παρεχόμενο αρχείο προορισμού. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | Αποθηκεύει το αρχείο στο αρχείο κατά διαδρομή με συμπίεση gzip. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | Αποθηκεύει το αρχείο στη ροή με συμπίεση xz. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | Αποθηκεύει το αρχείο στη διαδρομή ανά διαδρομή με συμπίεση xz. |

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* συνέλευση [Aspose.Zip](../../)


