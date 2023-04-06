---
title: Class Archive
second_title: Aspose.ZIP για Αναφορά API .NET
description: Aspose.Zip.Archive τάξη. Αυτή η κλάση αντιπροσωπεύει το αρχείο αρχείου zip. Χρησιμοποιήστε το για να συνθέσετε να εξαγάγετε ή να ενημερώσετε αρχεία zip.
type: docs
weight: 10
url: /el/net/aspose.zip/archive/
---
## Archive class

Αυτή η κλάση αντιπροσωπεύει το αρχείο αρχείου zip. Χρησιμοποιήστε το για να συνθέσετε, να εξαγάγετε ή να ενημερώσετε αρχεία zip.

```csharp
public class Archive : IArchive
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | Αρχικοποιεί μια νέα παρουσία του`Archive` τάξη με προαιρετικές ρυθμίσεις για τις καταχωρήσεις της. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | Αρχικοποιεί μια νέα παρουσία του`Archive` Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | Αρχικοποιεί μια νέα παρουσία του`Archive` Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Entries](../../aspose.zip/archive/entries/) { get; } | Λαμβάνει καταχωρήσεις του[`ArchiveEntry`](../archiveentry/) τύπος που αποτελεί το αρχείο. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για νέα προσθήκη[`ArchiveEntry`](../archiveentry/) αντικείμενα. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, Stream, ArchiveEntrySettings) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, FileInfo, bool, ArchiveEntrySettings) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, string, bool, ArchiveEntrySettings) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | Καταργεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρισης από τη λίστα καταχωρήσεων. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | Αφαιρεί την καταχώρηση από τη λίστα καταχωρήσεων κατά ευρετήριο. |
| [Dispose](../../aspose.zip/archive/dispose/)() | Εκτελεί εργασίες που καθορίζονται από την εφαρμογή που σχετίζονται με την απελευθέρωση, την απελευθέρωση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | Εξάγει όλα τα αρχεία στο αρχείο στον παρεχόμενο κατάλογο. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | Αποθηκεύει το αρχείο στη ροή που παρέχεται. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | Αποθηκεύει το αρχείο στο παρεχόμενο αρχείο προορισμού. |
| [SaveSplit](../../aspose.zip/archive/savesplit/)(string, SplitArchiveSaveOptions) | Αποθηκεύει το αρχείο πολλών τόμων στον παρεχόμενο κατάλογο προορισμού. |

### Δείτε επίσης

* interface [IArchive](../iarchive/)
* χώρος ονομάτων [Aspose.Zip](../../aspose.zip/)
* συνέλευση [Aspose.Zip](../../)


