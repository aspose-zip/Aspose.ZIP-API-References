---
title: "Κλάση SevenZipArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.SevenZip.SevenZipArchive κλάση. Αυτή η κλάση αντιπροσωπεύει αρχείο συμπιεσμένου 7z. Χρησιμοποιήστε την για τη σύνθεση και την εξαγωγή αρχείων 7z."
type: docs
weight: 1190
url: /el/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

Αυτή η κλάση αντιπροσωπεύει το αρχείο 7z. Χρησιμοποιήστε την για τη δημιουργία και την εξαγωγή αρχείων 7z.

```csharp
public class SevenZipArchive : IArchive
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `SevenZipArchive` με προαιρετικές ρυθμίσεις για τις καταχωρήσεις της. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream, SevenZipLoadOptions) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `SevenZipArchive` και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(Stream, string) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `SevenZipArchive` και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [SevenZipArchive](sevenziparchive/#constructor_3)(string, SevenZipLoadOptions) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `SevenZipArchive` και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [SevenZipArchive](sevenziparchive/#constructor_4)(string, string) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `SevenZipArchive` και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [SevenZipArchive](sevenziparchive/#constructor_5)(string[], string) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `SevenZipArchive` από πολυ‑τόμεο αρχείο 7z και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Λαμβάνει καταχωρήσεις του τύπου [`SevenZipArchiveEntry`](../sevenziparchiveentry/) που αποτελούν το αρχείο. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για τα πρόσφατα προστιθέμενα αντικείμενα [`SevenZipArchiveEntry`](../sevenziparchiveentry/). |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοθέντα κατάλογο. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοθέντα κατάλογο. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, Func&lt;Stream&gt;, SevenZipEntrySettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, FileInfo, bool, SevenZipEntrySettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_4)(string, string, bool, SevenZipEntrySettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Εκτελεί εργασίες ορισμένες από την εφαρμογή που σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Εξάγει όλα τα αρχεία στην αρχειοθήκη στον παρεχόμενο κατάλογο. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream, SevenZipArchiveSaveOptions) | Αποθηκεύει το αρχείο 7z στη δοθείσα ροή. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string, SevenZipArchiveSaveOptions) | Αποθηκεύει το αρχείο σε προορισμένο αρχείο που παρέχεται. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Αποθηκεύει το αρχείο πολλαπλών τόμων στον παρεχόμενο φάκελο προορισμού. |

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assembly [Aspose.Zip](../../)


