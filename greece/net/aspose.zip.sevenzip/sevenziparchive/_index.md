---
title: Class SevenZipArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: Aspose.Zip.SevenZip.SevenZipArchive τάξη. Αυτή η κλάση αντιπροσωπεύει αρχείο αρχειοθέτησης 7z. Χρησιμοποιήστε το για να συνθέσετε και να εξαγάγετε αρχεία 7z.
type: docs
weight: 660
url: /el/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

Αυτή η κλάση αντιπροσωπεύει αρχείο αρχειοθέτησης 7z. Χρησιμοποιήστε το για να συνθέσετε και να εξαγάγετε αρχεία 7z.

```csharp
public class SevenZipArchive : IArchive
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Αρχικοποιεί μια νέα παρουσία του`SevenZipArchive` τάξη με προαιρετικές ρυθμίσεις για τις καταχωρήσεις της. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | Αρχικοποιεί μια νέα παρουσία του`SevenZipArchive` Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | Αρχικοποιεί μια νέα παρουσία του`SevenZipArchive` Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Λαμβάνει καταχωρήσεις του[`SevenZipArchiveEntry`](../sevenziparchiveentry/) τύπος που αποτελεί το αρχείο. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για νέα προσθήκη[`SevenZipArchiveEntry`](../sevenziparchiveentry/) αντικείμενα. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | Δημιουργία μίας καταχώρησης μέσα στο αρχείο. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Εκτελεί εργασίες που καθορίζονται από την εφαρμογή που σχετίζονται με την απελευθέρωση, την απελευθέρωση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Εξάγει όλα τα αρχεία στο αρχείο στον παρεχόμενο κατάλογο. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | Αποθηκεύει το αρχείο 7z στην παρεχόμενη ροή. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | Αποθηκεύει το αρχείο στο παρεχόμενο αρχείο προορισμού. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Αποθηκεύει το αρχείο πολλών τόμων στον παρεχόμενο κατάλογο προορισμού. |

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* συνέλευση [Aspose.Zip](../../)


