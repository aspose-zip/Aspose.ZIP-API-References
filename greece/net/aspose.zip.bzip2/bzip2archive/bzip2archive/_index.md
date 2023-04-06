---
title: Bzip2Archive.Bzip2Archive
second_title: Aspose.ZIP για Αναφορά API .NET
description: Bzip2Archive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουBzip2Archive τάξη προετοιμασμένη για συμπίεση.
type: docs
weight: 10
url: /el/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`Bzip2Archive`](../) τάξη προετοιμασμένη για συμπίεση.

```csharp
public Bzip2Archive()
```

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Δείτε επίσης

* class [Bzip2Archive](../)
* χώρος ονομάτων [Aspose.Zip.Bzip2](../../bzip2archive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`Bzip2Archive`](../) τάξη προετοιμασμένη για αποσυμπίεση.

```csharp
public Bzip2Archive(Stream sourceStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζεται. Βλέπω[`Open`](../open/) μέθοδος αποσυμπίεσης.

### Παραδείγματα

Ανοίξτε ένα αρχείο από μια ροή και εξαγάγετε το σε ένα`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### Δείτε επίσης

* class [Bzip2Archive](../)
* χώρος ονομάτων [Aspose.Zip.Bzip2](../../bzip2archive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`Bzip2Archive`](../) τάξη προετοιμασμένη για αποσυμπίεση.

```csharp
public Bzip2Archive(string path)
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

Αυτός ο κατασκευαστής δεν αποσυμπιέζεται. Βλέπω[`Open`](../open/) μέθοδος αποσυμπίεσης.

### Παραδείγματα

Ανοίξτε ένα αρχείο από αρχείο προς διαδρομή και εξαγάγετε το στο a`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### Δείτε επίσης

* class [Bzip2Archive](../)
* χώρος ονομάτων [Aspose.Zip.Bzip2](../../bzip2archive/)
* συνέλευση [Aspose.Zip](../../../)


