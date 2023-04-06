---
title: Archive.ExtractToDirectory
second_title: Aspose.ZIP για Αναφορά API .NET
description: Archive μέθοδος. Εξάγει όλα τα αρχεία στο αρχείο στον παρεχόμενο κατάλογο.
type: docs
weight: 80
url: /el/net/aspose.zip/archive/extracttodirectory/
---
## Archive.ExtractToDirectory method

Εξάγει όλα τα αρχεία στο αρχείο στον παρεχόμενο κατάλογο.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | String | Η διαδρομή προς τον κατάλογο στον οποίο θα τοποθετηθούν τα εξαγόμενα αρχεία. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *destinationDirectory* είναι μηδενικό. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης στον υπάρχοντα κατάλογο. |
| NotSupportedException | Εάν ο κατάλογος δεν υπάρχει, η διαδρομή περιέχει έναν χαρακτήρα άνω και κάτω τελείας (:) που δεν αποτελεί μέρος μιας ετικέτας μονάδας δίσκου ("C:\"). |
| ArgumentException | *destinationDirectory*είναι μια συμβολοσειρά μηδενικού μήκους, περιέχει μόνο λευκό διάστημα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες. Μπορείτε να κάνετε ερώτημα για μη έγκυρους χαρακτήρες χρησιμοποιώντας τη μέθοδο System.IO.Path.GetInvalidPathChars. Η διαδρομή -or- έχει πρόθεμα ή περιέχει μόνο έναν χαρακτήρα άνω και κάτω τελείας (:). |
| IOException | Ο κατάλογος που καθορίζεται από τη διαδρομή είναι ένα αρχείο. -ή- Το όνομα του δικτύου δεν είναι γνωστό. |
| InvalidDataException | Έχει δοθεί λάθος κωδικός πρόσβασης. |

### Παρατηρήσεις

Εάν ο κατάλογος δεν υπάρχει, θα δημιουργηθεί.

### Παραδείγματα

```csharp
using (var archive = new Archive("archive.zip")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [Archive](../)
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)


