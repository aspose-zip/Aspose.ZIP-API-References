---
title: "Κλάση Archive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κλάση Aspose.Zip.Archive. Αυτή η κλάση αντιπροσωπεύει ένα αρχείο zip. Χρησιμοποιήστε την για να δημιουργήσετε, να εξάγετε ή να ενημερώσετε αρχεία zip."
type: docs
weight: 160
url: /el/net/aspose.zip/archive/
---
## Archive class

Αυτή η κλάση αναπαριστά ένα αρχείο zip. Χρησιμοποιήστε την για σύνθεση, εξαγωγή ή ενημέρωση αρχείων zip.

```csharp
public class Archive : IArchive
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης `Archive` με προαιρετικές ρυθμίσεις για τις καταχωρίσεις της. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης `Archive` και δημιουργεί μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από την αρχειοθήκη. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης `Archive` και δημιουργεί μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από την αρχειοθήκη. |
| [Archive](archive/#constructor_3)(string, string[], ArchiveLoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης `Archive` από πολυ-τόμευση αρχείο ZIP και δημιουργεί μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από την αρχειοθήκη. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Comment](../../aspose.zip/archive/comment/) { get; } | Λαμβάνει το σχόλιο για ολόκληρη την αρχειοθήκη. |
| [Entries](../../aspose.zip/archive/entries/) { get; } | Λαμβάνει τις καταχωρίσεις τύπου [`ArchiveEntry`](../archiveentry/) που αποτελούν την αρχειοθήκη. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για πρόσφατα προστιθέμενα στοιχεία [`ArchiveEntry`](../archiveentry/). |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | Προσθέτει στην αρχειοθήκη όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | Προσθέτει στην αρχειοθήκη όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, Func&lt;Stream&gt;, ArchiveEntrySettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, FileInfo, bool, ArchiveEntrySettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_4)(string, string, bool, ArchiveEntrySettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | Αφαιρεί την πρώτη εμφάνιση της συγκεκριμένης καταχώρησης από τη λίστα καταχωρίσεων. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | Αφαιρεί την καταχώρηση από τη λίστα καταχωρίσεων με βάση το δείκτη. |
| [Dispose](../../aspose.zip/archive/dispose/)() | Εκτελεί εργασίες ορισμένες από την εφαρμογή που σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | Εξάγει όλα τα αρχεία στην αρχειοθήκη στον παρεχόμενο κατάλογο. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | Αποθηκεύει την αρχειοθήκη στο παρεχόμενο αρχείο προορισμού |
| [SaveSplit](../../aspose.zip/archive/savesplit/#savesplit)(IVolumeStreamProvider, SplitArchiveSaveOptions) | Αποθηκεύει ένα αρχείο πολλαπλών τόμων σε ροές που παρέχονται από έναν πάροχο τόμων. |
| [SaveSplit](../../aspose.zip/archive/savesplit/#savesplit_1)(string, SplitArchiveSaveOptions) | Αποθηκεύει το αρχείο πολλαπλών τόμων στον παρεχόμενο φάκελο προορισμού. |

### Δείτε επίσης

* interface [IArchive](../iarchive/)
* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


