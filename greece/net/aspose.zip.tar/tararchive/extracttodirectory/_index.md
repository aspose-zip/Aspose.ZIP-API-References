---
title: "TarArchive.ExtractToDirectory"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος TarArchive. Εξάγει όλα τα αρχεία του αρχείου στον δοθέντα φάκελο."
type: docs
weight: 140
url: /el/net/aspose.zip.tar/tararchive/extracttodirectory/
---
## TarArchive.ExtractToDirectory method

Εξάγει όλα τα αρχεία στην αρχειοθήκη στον παρεχόμενο κατάλογο.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | String | Η διαδρομή προς το φάκελο όπου θα τοποθετηθούν τα εξαγόμενα αρχεία. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | Το Path είναι null |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| SecurityException | Ο καλών δεν διαθέτει τα απαιτούμενα δικαιώματα για πρόσβαση στον υπάρχον φάκελο. |
| NotSupportedException | Εάν ο φάκελος δεν υπάρχει, η διαδρομή περιέχει χαρακτήρα άνω-κάθετο (:) που δεν αποτελεί μέρος ετικέτας μονάδας (\"C:\\"). |
| ArgumentException | Το Path είναι μια συμβολοσειρά μηδενικού μήκους, περιέχει μόνο κενά διαστήματα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες. Μπορείτε να ελέγξετε για μη έγκυρους χαρακτήρες χρησιμοποιώντας τη μέθοδο System.IO.Path.GetInvalidPathChars. - ή - το path έχει πρόθεμα ή περιέχει μόνο το χαρακτήρα άνω-κάτω (:). |
| IOException | Ο φάκελος που καθορίστηκε από το path είναι αρχείο. - ή - Το όνομα δικτύου δεν είναι γνωστό. |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί και δεν μπορεί να χρησιμοποιηθεί |

## Παρατηρήσεις

Εάν ο φάκελος δεν υπάρχει, θα δημιουργηθεί.

## Παραδείγματα

```csharp
Using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


