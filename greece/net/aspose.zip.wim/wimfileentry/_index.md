---
title: "Κλάση WimFileEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.Wim.WimFileEntry κλάση. Αντιπροσωπεύει ένα μόνο αρχείο μέσα σε αρχείο wim"
type: docs
weight: 1360
url: /el/net/aspose.zip.wim/wimfileentry/
---
## WimFileEntry class

Αντιπροσωπεύει ένα μοναδικό αρχείο μέσα στην αρχειοθήκη wim.

```csharp
public sealed class WimFileEntry : WimEntry, IArchiveFileEntry
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams/) { get; } | Λαμβάνει τα ονόματα των εναλλακτικών ροών δεδομένων για ένα αρχείο ή φάκελο. |
| [Archive](../../aspose.zip.wim/wimentry/archive/) { get; } | Λαμβάνει το αρχείο στο οποίο ανήκει η καταχώρηση. |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime/) { get; } | Λαμβάνει την τελευταία φορά που το αρχείο ή ο φάκελος άλλαξε. |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime/) { get; } | Λαμβάνει την ώρα δημιουργίας του αρχείου ή του φακέλου. |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes/) { get; } | Λαμβάνει τα χαρακτηριστικά του αρχείου ή του φακέλου. |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath/) { get; } | Λαμβάνει μια πλήρη διαδρομή της καταχώρησης μέσα στην εικόνα. |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink/) { get; } | Λαμβάνει το αναγνωριστικό hardlink του αρχείου ή του φακέλου. |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks/) { get; } | Λαμβάνει εάν το αρχείο ή ο φάκελος είναι γνωστό με άλλα ονόματα. |
| [Image](../../aspose.zip.wim/wimentry/image/) { get; } | Λαμβάνει την εικόνα στην οποία ανήκει η καταχώρηση. |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory/) { get; } | Επιστρέφει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο. |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime/) { get; } | Λαμβάνει την τελευταία ώρα πρόσβασης του αρχείου ή του φακέλου. |
| [Length](../../aspose.zip.wim/wimfileentry/length/) { get; } | Λαμβάνει το μήκος της καταχώρησης σε byte. |
| [ModificationTime](../../aspose.zip.wim/wimentry/modificationtime/) { get; } | Λαμβάνει την ώρα τροποποίησης του αρχείου ή του καταλόγου. |
| [Name](../../aspose.zip.wim/wimentry/name/) { get; } | Λαμβάνει το όνομα της καταχώρησης μέσα στην εικόνα. |
| [Parent](../../aspose.zip.wim/wimentry/parent/) { get; } | Λαμβάνει τον γονικό φάκελο στον οποίο ανήκει η καταχώρηση. |
| [ShortName](../../aspose.zip.wim/wimentry/shortname/) { get; } | Λαμβάνει το σύντομο όνομα της καταχώρησης μέσα στην εικόνα. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract_1)(Stream) | Εξάγει την καταχώρηση στη δοθείσα ροή. |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract)(string) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη δοθείσα διαδρομή. |
| [Open](../../aspose.zip.wim/wimfileentry/open/)() | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει ένα ρεύμα με το περιεχόμενο της καταχώρησης. |
| override [ToString](../../aspose.zip.wim/wimentry/tostring/)() |  |

### Δείτε επίσης

* class [WimEntry](../wimentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Wim](../../aspose.zip.wim/)
* assembly [Aspose.Zip](../../)


