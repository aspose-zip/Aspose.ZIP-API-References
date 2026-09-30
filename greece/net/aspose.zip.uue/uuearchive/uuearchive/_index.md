---
title: "UueArchive.UueArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "UueArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία της κλάσης UueArchive προετοιμασμένη για κωδικοποίηση"
type: docs
weight: 10
url: /el/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`UueArchive`](../) προετοιμασμένη για κωδικοποίηση.

```csharp
public UueArchive()
```

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να κωδικοποιήσετε ένα αρχείο με uuencode.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### Δείτε επίσης

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`UueArchive`](../) προετοιμασμένη για αποκωδικοποίηση.

```csharp
public UueArchive(Stream sourceStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποκωδικοποιεί. Δείτε τη μέθοδο [`Open`](../open/) για αποσυμπίεση.

## Παραδείγματα

Ανοίξτε ένα αρχείο από μια ροή και εξάγετέ το σε ένα `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### Δείτε επίσης

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`UueArchive`](../).

```csharp
public UueArchive(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο αρχειοθήκης. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Open`](../open/) για αποσυμπίεση.

## Παραδείγματα

Ανοίξτε ένα αρχείο από το αρχείο με διαδρομή και αποκωδικοποιήστε το σε ένα `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### Δείτε επίσης

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


