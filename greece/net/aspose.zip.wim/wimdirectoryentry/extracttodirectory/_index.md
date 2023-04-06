---
title: WimDirectoryEntry.ExtractToDirectory
second_title: Aspose.ZIP για Αναφορά API .NET
description: WimDirectoryEntry μέθοδος. Εξάγει όλα τα αρχεία στον τρέχοντα κατάλογο στον παρεχόμενο κατάλογο.
type: docs
weight: 50
url: /el/net/aspose.zip.wim/wimdirectoryentry/extracttodirectory/
---
## WimDirectoryEntry.ExtractToDirectory method

Εξάγει όλα τα αρχεία στον τρέχοντα κατάλογο στον παρεχόμενο κατάλογο.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | String | Η διαδρομή προς τον κατάλογο στον οποίο θα τοποθετηθούν τα εξαγόμενα αρχεία. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | η διαδρομή είναι μηδενική |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης στον υπάρχοντα κατάλογο. |
| NotSupportedException | Εάν ο κατάλογος δεν υπάρχει, η διαδρομή περιέχει έναν χαρακτήρα άνω και κάτω τελείας (:) που δεν αποτελεί μέρος μιας ετικέτας μονάδας δίσκου ("C:\"). |
| ArgumentException | Η διαδρομή είναι μια συμβολοσειρά μηδενικού μήκους, περιέχει μόνο λευκό διάστημα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες. Μπορείτε να κάνετε ερώτημα για μη έγκυρους χαρακτήρες χρησιμοποιώντας τη μέθοδο System.IO.Path.GetInvalidPathChars. Το -or- path έχει πρόθεμα ή περιέχει μόνο έναν χαρακτήρα άνω και κάτω τελείας (:). |
| IOException | Ο κατάλογος που καθορίζεται από τη διαδρομή είναι ένα αρχείο. -ή- Το όνομα του δικτύου δεν είναι γνωστό. |

### Παρατηρήσεις

Εάν ο κατάλογος δεν υπάρχει, θα δημιουργηθεί.

### Παραδείγματα

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].RootDirectory.ExtractToDirectory(@"C:\\extracted");
}
```

### Δείτε επίσης

* class [WimDirectoryEntry](../)
* χώρος ονομάτων [Aspose.Zip.Wim](../../wimdirectoryentry/)
* συνέλευση [Aspose.Zip](../../../)


