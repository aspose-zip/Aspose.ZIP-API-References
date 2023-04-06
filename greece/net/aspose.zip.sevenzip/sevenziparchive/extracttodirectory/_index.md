---
title: SevenZipArchive.ExtractToDirectory
second_title: Aspose.ZIP για Αναφορά API .NET
description: SevenZipArchive μέθοδος. Εξάγει όλα τα αρχεία στο αρχείο στον παρεχόμενο κατάλογο.
type: docs
weight: 70
url: /el/net/aspose.zip.sevenzip/sevenziparchive/extracttodirectory/
---
## SevenZipArchive.ExtractToDirectory method

Εξάγει όλα τα αρχεία στο αρχείο στον παρεχόμενο κατάλογο.

```csharp
public void ExtractToDirectory(string destinationDirectory, string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | String | Η διαδρομή προς τον κατάλογο στον οποίο θα τοποθετηθούν τα εξαγόμενα αρχεία. |
| password | String | Προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *destinationDirectory* είναι μηδενικό. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης στον υπάρχοντα κατάλογο. |
| NotSupportedException | Εάν ο κατάλογος δεν υπάρχει, η διαδρομή περιέχει έναν χαρακτήρα άνω και κάτω τελείας (:) που δεν αποτελεί μέρος μιας ετικέτας μονάδας δίσκου ("C:\"). |
| ArgumentException | *destinationDirectory* είναι μια συμβολοσειρά μηδενικού μήκους, περιέχει μόνο λευκό διάστημα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες. Μπορείτε να κάνετε ερώτημα για μη έγκυρους χαρακτήρες χρησιμοποιώντας τη μέθοδο System.IO.Path.GetInvalidPathChars. Το -or- path έχει πρόθεμα ή περιέχει μόνο έναν χαρακτήρα άνω και κάτω τελείας (:). |
| IOException | Ο κατάλογος που καθορίζεται από τη διαδρομή είναι ένα αρχείο. -ή- Το όνομα του δικτύου δεν είναι γνωστό. |

### Παρατηρήσεις

Εάν ο κατάλογος δεν υπάρχει, θα δημιουργηθεί.

### Παραδείγματα

```csharp
using (var archive = new SevenZipArchive("archive.7z")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [SevenZipArchive](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)

