---
title: "ArchiveFactory.CompressDirectory"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος ArchiveFactory. Συμπιέζει τον καθορισμένο φάκελο σε αρχείο χρησιμοποιώντας τη δοθείσα μορφή αρχείου."
type: docs
weight: 10
url: /el/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

Συμπιέζει τον καθορισμένο κατάλογο σε αρχείο συμπιεσμένου αρχείου χρησιμοποιώντας τη δοθείσα μορφή αρχείου.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Το μονοπάτι προς το φάκελο που θα συμπιεστεί. |
| outputFileName | String | Όνομα αρχείου προορισμού. |
| archiveFormat | ArchiveFormat | Η μορφή του αρχείου που θα δημιουργηθεί (π.χ., zip, rar, tar, κλπ.). |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| DirectoryNotFoundException | Δημιουργείται εάν ο φάκελος που καθορίζεται από *path* δεν υπάρχει. |
| ArgumentException | Δημιουργείται εάν *path* είναι null ή κενή συμβολοσειρά. |
| NotSupportedException | Δημιουργείται εάν η καθορισμένη *archiveFormat* δεν υποστηρίζεται ή δεν αναγνωρίζεται. |
| ArgumentNullException | *path* είναι `null`. |

## Παρατηρήσεις

Αυτή η μέθοδος θα δημιουργήσει ένα αρχείο αρχειοθήκης στη θέση που καθορίζεται από την παράμετρο *path*. Το όνομα του αρχείου αρχειοθήκης συνήθως θα είναι το όνομα του καταλόγου ακολουθούμενο από την κατάλληλη επέκταση αρχείου βάσει του *archiveFormat*. Ο ίδιος ο κατάλογος δεν τροποποιείται ούτε διαγράφεται.

## Παραδείγματα

Ακολουθεί ένα παράδειγμα για το πώς να χρησιμοποιήσετε τη μέθοδο CompressDirectory:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// Αυτό θα δημιουργήσει ένα αρχείο ZIP με το περιεχόμενο του καταλόγου στη καθορισμένη διαδρομή.
```

### Δείτε επίσης

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


