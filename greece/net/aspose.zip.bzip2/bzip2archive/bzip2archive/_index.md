---
title: "Bzip2Archive.Bzip2Archive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής Bzip2Archive. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης Bzip2Archive προετοιμασμένο για συμπίεση"
type: docs
weight: 10
url: /el/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Bzip2Archive`](../) προετοιμασμένο για συμπίεση.

```csharp
public Bzip2Archive()
```

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Δείτε επίσης

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream, Bzip2LoadOptions) {#constructor_1}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Bzip2Archive`](../) προετοιμασμένο για αποσυμπίεση.

```csharp
public Bzip2Archive(Stream sourceStream, Bzip2LoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| loadOptions | Bzip2LoadOptions | Οι επιλογές για τη φόρτωση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| EndOfStreamException | Πρόωρος τερματισμός ροής. |
| InvalidDataException | Λάθος bytes υπογραφής. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |
| ArgumentNullException | *sourceStream* είναι null. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Open`](../open/) για αποσυμπίεση.

## Παραδείγματα

Ανοίξτε ένα αρχείο από μια ροή και εξάγετέ το σε ένα `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### Δείτε επίσης

* class [Bzip2LoadOptions](../../bzip2loadoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2Archive(string, Bzip2LoadOptions) {#constructor_2}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Bzip2Archive`](../) προετοιμασμένο για αποσυμπίεση.

```csharp
public Bzip2Archive(string path, Bzip2LoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο αρχειοθήκης. |
| loadOptions | Bzip2LoadOptions | Οι επιλογές για τη φόρτωση του αρχείου. |

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
| EndOfStreamException | Πρόωρος τερματισμός ροής. |
| InvalidDataException | Λάθος bytes υπογραφής. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Open`](../open/) για αποσυμπίεση.

## Παραδείγματα

Ανοίξτε ένα αρχείο από διαδρομή και εξάγετε το σε ένα `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### Δείτε επίσης

* class [Bzip2LoadOptions](../../bzip2loadoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


