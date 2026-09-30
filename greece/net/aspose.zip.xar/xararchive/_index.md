---
title: "Κλάση XarArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.Xar.XarArchive class. Αυτή η κλάση αντιπροσωπεύει ένα αρχείο xar"
type: docs
weight: 1420
url: /el/net/aspose.zip.xar/xararchive/
---
## XarArchive class

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο αρχειοθήκης xar.

```csharp
public class XarArchive : IArchive
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [XarArchive](xararchive/#constructor)(XarCompressionSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης `XarArchive`. |
| [XarArchive](xararchive/#constructor_1)(Stream, XarLoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης `XarArchive` και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [XarArchive](xararchive/#constructor_2)(string, XarLoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης `XarArchive` και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Entries](../../aspose.zip.xar/xararchive/entries/) { get; } | Λαμβάνει καταχωρήσεις τύπου [`XarEntry`](../xarentry/) που αποτελούν το αρχείο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CreateEntries](../../aspose.zip.xar/xararchive/createentries/#createentries)(DirectoryInfo, bool, XarCompressionSettings) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά από τον δοσμένο κατάλογο. |
| [CreateEntries](../../aspose.zip.xar/xararchive/createentries/#createentries_1)(string, bool, XarCompressionSettings) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά από τον δοσμένο κατάλογο. |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry_1)(string, Stream, XarCompressionSettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry)(string, FileInfo, bool, XarCompressionSettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry_2)(string, string, bool, XarCompressionSettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [DeleteEntry](../../aspose.zip.xar/xararchive/deleteentry/)(XarEntry) | Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων. |
| [Dispose](../../aspose.zip.xar/xararchive/dispose/)() | Εκτελεί εργασίες ορισμένες από την εφαρμογή που σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip.xar/xararchive/extracttodirectory/)(string) | Εξάγει όλα τα αρχεία στην αρχειοθήκη στον παρεχόμενο κατάλογο. |
| [Save](../../aspose.zip.xar/xararchive/save/#save)(Stream, XarSaveOptions) | Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή. |
| [Save](../../aspose.zip.xar/xararchive/save/#save_1)(string, XarSaveOptions) | Αποθηκεύει την αρχειοθήκη στο παρεχόμενο αρχείο προορισμού |

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assembly [Aspose.Zip](../../)


