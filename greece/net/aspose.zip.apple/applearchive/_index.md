---
title: "Κλάση AppleArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.Apple.AppleArchive κλάση. Αυτή η κλάση αντιπροσωπεύει ένα αρχείο Apple Archive .aar. Χρησιμοποιήστε το για να δημιουργήσετε αρχεία Apple Archive"
type: docs
weight: 60
url: /el/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο Apple Archive (.aar). Χρησιμοποιήστε την για τη δημιουργία αρχείων Apple Archive.

```csharp
public class AppleArchive : IArchive
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης `AppleArchive` με τις ρυθμίσεις που χρησιμοποιούνται για τις συντεθειμένες καταχωρίσεις |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης `AppleArchive` και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης `AppleArchive` και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | Λαμβάνει τις καταχωρίσεις που αποτελούν το αρχείο |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν το αρχείο χρησιμοποιεί συμπίεση solid. Σε λειτουργία solid, όλα τα δεδομένα των καταχωρίσεων συμπιέζονται ως ένα ενιαίο ρεύμα και η ατομική εξαγωγή καταχωρίσεων δεν είναι διαθέσιμη. Χρησιμοποιήστε το [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/) αντ' αυτού |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | Λαμβάνει τις ρυθμίσεις που χρησιμοποιούνται για τις νεοσυντεθειμένες καταχωρίσεις |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοθέντα κατάλογο. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | Εκτελεί εργασίες ορισμένες από την εφαρμογή που σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | Εξάγει όλα τα αρχεία στην αρχειοθήκη στον παρεχόμενο κατάλογο. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | Αποθηκεύει το αρχείο σε προορισμένο αρχείο που παρέχεται. |

## Παρατηρήσεις

Apple και Apple Archive είναι εμπορικά σήματα της Apple Inc.

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


