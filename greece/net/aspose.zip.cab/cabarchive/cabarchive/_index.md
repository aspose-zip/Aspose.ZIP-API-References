---
title: CabArchive.CabArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: CabArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουCabArchive Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.
type: docs
weight: 10
url: /el/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(Stream) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`CabArchive`](../) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.

```csharp
public CabArchive(Stream sourceStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. Πρέπει να είναι αναζητήσιμο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *sourceStream* είναι μηδενικό. |
| ArgumentException | *sourceStream* δεν είναι αναζητήσιμο. |
| InvalidDataException | *sourceStream* δεν είναι έγκυρο αρχείο ταξί. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυσκευάζει καμία καταχώρηση. Βλέπω[`Open`](../../cabentry/open/)μέθοδος αποσυσκευασίας.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε όλες τις εγγραφές σε έναν κατάλογο.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [CabArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cab](../../cabarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CabArchive(string) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`CabArchive`](../) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.

```csharp
public CabArchive(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η διαδρομή προς το αρχείο αρχειοθέτησης. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *path* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*path* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*path* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*path*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*path* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυσκευάζει καμία καταχώρηση. Βλέπω[`Open`](../../cabentry/open/)μέθοδος αποσυσκευασίας.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε όλες τις εγγραφές σε έναν κατάλογο.

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


