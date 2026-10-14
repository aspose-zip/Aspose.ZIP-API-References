---
title: "RarArchive.ExtractToDirectory"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος RarArchive. Εξάγει όλα τα αρχεία του αρχείου στον παρεχόμενο φάκελο"
type: docs
weight: 40
url: /el/net/aspose.zip.rar/rararchive/extracttodirectory/
---
## RarArchive.ExtractToDirectory method

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
| ArgumentNullException | *destinationDirectory* είναι null. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| SecurityException | Ο καλών δεν διαθέτει τα απαιτούμενα δικαιώματα για πρόσβαση στον υπάρχον φάκελο. |
| NotSupportedException | Εάν ο φάκελος δεν υπάρχει, η διαδρομή περιέχει χαρακτήρα άνω-κάθετο (:) που δεν αποτελεί μέρος ετικέτας μονάδας (\"C:\\"). |
| ArgumentException | *destinationDirectory* είναι συμβολοσειρά μηδενικού μήκους, περιέχει μόνο κενά διαστήματα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες. Μπορείτε να ερωτήσετε για μη έγκυρους χαρακτήρες χρησιμοποιώντας τη μέθοδο System.IO.Path.GetInvalidPathChars. -or- η διαδρομή προέρχεται ή περιέχει μόνο χαρακτήρα άνω-κάθετο (:). |
| IOException | Ο φάκελος που καθορίζεται από τη διαδρομή είναι αρχείο. -or- Το όνομα δικτύου είναι άγνωστο. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παρατηρήσεις

Εάν ο φάκελος δεν υπάρχει, θα δημιουργηθεί.

Για την εξαγωγή κρυπτογραφημένου `RarArchive` χρησιμοποιήστε το [`DecryptionPassword`](../../rararchiveloadoptions/decryptionpassword/)

## Παραδείγματα

```csharp
using (var archive = new RarArchive("archive.rar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [RarArchive](../)
* namespace [Aspose.Zip.Rar](../../rararchive/)
* assembly [Aspose.Zip](../../../)


