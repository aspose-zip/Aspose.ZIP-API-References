---
title: "LzxArchive.LzxArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής LzxArchive. Αρχικοποιεί μια νέα παρουσία της κλάσης LzxArchive και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο."
type: docs
weight: 10
url: /el/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LzxArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| extractionSource | Stream | Η πηγή του αρχείου. |
| loadOptions | LzxLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *extractionSource* είναι null. |
| ArgumentException | *extractionSource* δεν υποστηρίζει αναζήτηση. |
| InvalidDataException | Λάθος υπογραφή για το αρχείο. - ή - Το αρχείο δεν είναι αρχείο LZX. |
| NotImplementedException | Το αρχείο Lzx περιέχει συγχωνευμένες καταχωρήσεις. |
| EndOfStreamException | Η ροή *extractionSource* είναι πολύ σύντομη. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή έχει κλείσει. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Extract`](../../lzxarchiveentry/extract/) για αποσυμπίεση.

### Δείτε επίσης

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LzxArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η πλήρης ή σχετική διαδρομή προς το αρχείο του αρχείου. |
| loadOptions | LzxLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

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
| InvalidDataException | Το αρχείο είναι κατεστραμμένο. |
| NotImplementedException | Το αρχείο Lzx περιέχει συγχωνευμένες καταχωρήσεις. |
| EndOfStreamException | Το αρχείο είναι πολύ μικρό. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή έχει κλείσει. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Extract`](../../lzxarchiveentry/extract/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα εξάγει ένα αρχείο, στη συνέχεια αποσυμπιέζει την πρώτη καταχώρηση σε ένα `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Δείτε επίσης

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


