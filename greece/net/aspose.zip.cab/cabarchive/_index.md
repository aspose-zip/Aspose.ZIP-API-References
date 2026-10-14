---
title: "Κλάση CabArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.Cab.CabArchive κλάση. Αυτή η κλάση αντιπροσωπεύει ένα αρχείο CAB."
type: docs
weight: 310
url: /el/net/aspose.zip.cab/cabarchive/
---
## CabArchive class

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο CAB.

```csharp
public class CabArchive : IArchive
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [CabArchive](cabarchive/#constructor)(CabEntrySettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης `CabArchive` προετοιμασμένη για συμπίεση. |
| [CabArchive](cabarchive/#constructor_1)(Stream, CabLoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης `CabArchive` και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [CabArchive](cabarchive/#constructor_2)(string, CabLoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης `CabArchive` και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Entries](../../aspose.zip.cab/cabarchive/entries/) { get; } | Λαμβάνει καταχωρήσεις τύπου [`CabEntry`](../cabentry/) που αποτελούν το αρχείο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CreateEntries](../../aspose.zip.cab/cabarchive/createentries/#createentries)(DirectoryInfo, bool) | Προσθέτει στο αρχείο όλα τα αρχεία, αναδρομικά, από τον καθορισμένο φάκελο. |
| [CreateEntries](../../aspose.zip.cab/cabarchive/createentries/#createentries_1)(string, bool) | Προσθέτει στο αρχείο όλα τα αρχεία αναδρομικά από τη διαδρομή του καθορισμένου φακέλου. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_1)(string, FileInfo, CabEntrySettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry)(string, Func&lt;Stream&gt;, CabEntrySettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_2)(string, Stream, CabEntrySettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_3)(string, string, CabEntrySettings) | Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη. |
| [Dispose](../../aspose.zip.cab/cabarchive/dispose/)() | Εκτελεί εργασίες ορισμένες από την εφαρμογή που σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip.cab/cabarchive/extracttodirectory/)(string) | Εξάγει όλα τα αρχεία στην αρχειοθήκη στον παρεχόμενο κατάλογο. |
| [Save](../../aspose.zip.cab/cabarchive/save/#save)(Stream, CabSaveOptions) | Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή. |
| [Save](../../aspose.zip.cab/cabarchive/save/#save_1)(string, CabSaveOptions) | Αποθηκεύει την αρχειοθήκη στο παρεχόμενο αρχείο προορισμού |

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Cab](../../aspose.zip.cab/)
* assembly [Aspose.Zip](../../)


