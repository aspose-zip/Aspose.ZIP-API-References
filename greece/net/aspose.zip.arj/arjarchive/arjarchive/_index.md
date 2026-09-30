---
title: "ArjArchive.ArjArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής ArjArchive. Δημιουργεί ένα νέο αντικείμενο της κλάσης ArjArchive και συνθέτει μια λίστα καταχωρίσεων που μπορούν να εξαχθούν από το αρχείο"
type: docs
weight: 10
url: /el/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

Δημιουργεί ένα νέο αντικείμενο της κλάσης [`ArjArchive`](../) και συνθέτει μια λίστα καταχωρίσεων που μπορούν να εξαχθούν από το αρχείο.

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| extractionSource | Stream | Η πηγή του αρχείου. |
| loadOptions | ArjLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *extractionSource* είναι null. |
| ArgumentException | &gt;*extractionSource* δεν υποστηρίζει αναζήτηση. |
| InvalidDataException | Λάθος υπογραφή για το αρχείο. - ή - Το αρχείο δεν είναι αρχείο ARJ. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν όλα τα byte της κεφαλίδας ή του ονόματος. |
| NotSupportedException | Το αρχείο είναι κατεστραμμένο. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Extract`](../../arjentryplain/extract/) για αποσυμπίεση.

### Δείτε επίσης

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

Δημιουργεί ένα νέο αντικείμενο της κλάσης [`ArjArchive`](../) και συνθέτει μια λίστα καταχωρίσεων που μπορούν να εξαχθούν από το αρχείο.

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο αρχειοθήκης. |
| loadOptions | ArjLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

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
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν όλα τα byte της κεφαλίδας ή του ονόματος. |
| InvalidDataException | Ο μαγικός αριθμός ARJ είναι άκυρος ή το μέγεθος της κεφαλίδας είναι εκτός εύρους. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Extract`](../../arjentryplain/extract/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


