---
title: "Κλάση XarFileEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.Xar.XarFileEntry κλάση. Αντιπροσωπεύει καταχώρηση αρχείου μέσα σε αρχειοθήκη xar."
type: docs
weight: 1470
url: /el/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

Αντιπροσωπεύει την καταχώρηση αρχείου μέσα σε αρχειοθήκη xar.

```csharp
public sealed class XarFileEntry : XarEntry, IArchiveFileEntry
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | Λαμβάνει την ώρα δημιουργίας του αρχείου ή του φακέλου. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | Λαμβάνει την πλήρη διαδρομή της καταχώρησης μέσα στην αρχειοθήκη. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | Επιστρέφει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | Λαμβάνει την τελευταία ώρα πρόσβασης του αρχείου ή του φακέλου. |
| [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | Λαμβάνει το μήκος της καταχώρησης σε byte. |
| [ModificationTime](../../aspose.zip.xar/xarentry/modificationtime/) { get; } | Λαμβάνει την ώρα τροποποίησης του αρχείου ή του καταλόγου. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | Επιστρέφει το όνομα της καταχώρησης μέσα στο αρχείο. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | Λαμβάνει τον γονικό φάκελο στον οποίο ανήκει η καταχώρηση. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | Εξάγει την καταχώρηση στη δοθείσα ροή. |
| [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη δοθείσα διαδρομή. |
| [Open](../../aspose.zip.xar/xarfileentry/open/)() | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει ένα ρεύμα με το περιεχόμενο της καταχώρησης. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

## Συμβάντα

| Όνομα | Περιγραφή |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.xar/xarfileentry/compressionprogressed/) | Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής συμπιέζεται. |

### Δείτε επίσης

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assembly [Aspose.Zip](../../)


