---
title: "SnappyArchive.SnappyArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής SnappyArchive. Αρχικοποιεί μια νέα παρουσία της κλάσης SnappyArchive προετοιμασμένη για συμπίεση"
type: docs
weight: 10
url: /el/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`SnappyArchive`](../) προετοιμασμένη για συμπίεση.

```csharp
public SnappyArchive()
```

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snappy");
}
```

### Δείτε επίσης

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`SnappyArchive`](../) προετοιμασμένη για αποσυμπίεση.

```csharp
public SnappyArchive(Stream source)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | Stream | Η πηγή του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *source* δεν είναι δυνατόν να γίνει αναζήτηση. |
| ArgumentNullException | *source* είναι null. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Extract`](../extract/) για αποσυμπίεση.

### Δείτε επίσης

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`SnappyArchive`](../) προετοιμασμένη για αποσυμπίεση.

```csharp
public SnappyArchive(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Διαδρομή προς την πηγή του αρχείου. |

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

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Extract`](../extract/) για αποσυμπίεση.

## Παραδείγματα

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
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)


