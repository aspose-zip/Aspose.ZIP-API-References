---
title: SnappyArchive.SnappyArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: SnappyArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουSnappyArchive τάξη προετοιμασμένη για συμπίεση.
type: docs
weight: 10
url: /el/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`SnappyArchive`](../) τάξη προετοιμασμένη για συμπίεση.

```csharp
public SnappyArchive()
```

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snapy");
}
```

### Δείτε επίσης

* class [SnappyArchive](../)
* χώρος ονομάτων [Aspose.Zip.Snappy](../../snappyarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`SnappyArchive`](../) τάξη προετοιμασμένη για αποσυμπίεση.

```csharp
public SnappyArchive(Stream source)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | Stream | Η πηγή του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *source* δεν είναι αναζητήσιμο. |
| ArgumentNullException | *source* είναι μηδενικό. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζεται. Βλέπω[`Extract`](../extract/) μέθοδος αποσυμπίεσης.

### Δείτε επίσης

* class [SnappyArchive](../)
* χώρος ονομάτων [Aspose.Zip.Snappy](../../snappyarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`SnappyArchive`](../) τάξη προετοιμασμένη για αποσυμπίεση.

```csharp
public SnappyArchive(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Διαδρομή προς την πηγή του αρχείου. |

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

Αυτός ο κατασκευαστής δεν αποσυμπιέζεται. Βλέπω[`Extract`](../extract/) μέθοδος αποσυμπίεσης.

### Παραδείγματα

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new SnappyArchive(sourceSnappyFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Δείτε επίσης

* class [SnappyArchive](../)
* χώρος ονομάτων [Aspose.Zip.Snappy](../../snappyarchive/)
* συνέλευση [Aspose.Zip](../../../)


