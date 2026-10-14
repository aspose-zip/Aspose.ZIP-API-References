---
title: "WimArchive.WimArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "WimArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία της κλάσης WimArchive και συνθέτει μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο"
type: docs
weight: 10
url: /el/net/aspose.zip.wim/wimarchive/wimarchive/
---
## WimArchive(Stream, WimLoadOptions) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`WimArchive`](../) και συνθέτει μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

```csharp
public WimArchive(Stream sourceStream, WimLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. Πρέπει να είναι δυνατότητα αναζήτησης. |
| loadOptions | WimLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *sourceStream* είναι null. |
| ArgumentException | *sourceStream* δεν είναι δυνατόν να γίνει αναζήτηση. |
| InvalidDataException | *sourceStream* δεν είναι έγκυρο αρχείο wim. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |
| NotSupportedException | Η κεφαλίδα υποδεικνύει αρχείο πολλαπλών τμημάτων. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Open`](../../wimfileentry/open/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο.

```csharp
using (var archive = new WimArchive(File.OpenRead("archive.wim")))
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [WimLoadOptions](../../wimloadoptions/)
* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)

---

## WimArchive(string, WimLoadOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`WimArchive`](../) και συνθέτει μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

```csharp
public WimArchive(string path, WimLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο αρχειοθήκης. |
| loadOptions | WimLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| InvalidDataException | Η κεφαλίδα υποδεικνύει αρχείο πολλαπλών τμημάτων. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Open`](../../wimfileentry/open/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο.

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [WimLoadOptions](../../wimloadoptions/)
* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)


