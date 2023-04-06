---
title: CabArchive.ExtractToDirectory
second_title: Aspose.ZIP για Αναφορά API .NET
description: CabArchive μέθοδος. Εξάγει όλα τα αρχεία στο αρχείο στον παρεχόμενο κατάλογο.
type: docs
weight: 40
url: /el/net/aspose.zip.cab/cabarchive/extracttodirectory/
---
## CabArchive.ExtractToDirectory method

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
| ArgumentNullException | η διαδρομή είναι μηδενική |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης στον υπάρχοντα κατάλογο. |
| NotSupportedException | Εάν ο κατάλογος δεν υπάρχει, η διαδρομή περιέχει έναν χαρακτήρα άνω και κάτω τελείας (:) που δεν αποτελεί μέρος μιας ετικέτας μονάδας δίσκου ("C:\"). |
| ArgumentException | Η διαδρομή είναι μια συμβολοσειρά μηδενικού μήκους, περιέχει μόνο λευκό διάστημα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες. Μπορείτε να κάνετε ερώτημα για μη έγκυρους χαρακτήρες χρησιμοποιώντας τη μέθοδο System.IO.Path.GetInvalidPathChars. Το -or- path έχει πρόθεμα ή περιέχει μόνο έναν χαρακτήρα άνω και κάτω τελείας (:). |
| IOException | Ο κατάλογος που καθορίζεται από τη διαδρομή είναι ένα αρχείο. -ή- Το όνομα του δικτύου δεν είναι γνωστό. |

### Παρατηρήσεις

Εάν ο κατάλογος δεν υπάρχει, θα δημιουργηθεί.

### Παραδείγματα

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [CabArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cab](../../cabarchive/)
* συνέλευση [Aspose.Zip](../../../)


