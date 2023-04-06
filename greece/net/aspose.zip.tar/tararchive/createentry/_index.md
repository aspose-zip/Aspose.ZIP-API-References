---
title: TarArchive.CreateEntry
second_title: Aspose.ZIP για Αναφορά API .NET
description: TarArchive μέθοδος. Δημιουργία μίας καταχώρησης μέσα στο αρχείο.
type: docs
weight: 80
url: /el/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |
| fileInfo | FileSystemInfo | Τα μεταδεδομένα του αρχείου ή του φακέλου που πρόκειται να συμπιεστούν. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής πίσσας.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| PathTooLongException | *name* είναι πολύ μεγάλη για την πίσσα από το πρότυπο IEEE 1003.1-1998. |
| ArgumentException | Όνομα αρχείου, ως μέρος του*name*, υπερβαίνει τα 100 σύμβολα. |

### Παρατηρήσεις

Το όνομα καταχώρισης ορίζεται αποκλειστικά μέσα*name* παράμετρος. Το όνομα αρχείου που παρέχεται*fileInfo* η παράμετρος δεν επηρεάζει το όνομα της καταχώρισης.

*fileInfo* μπορεί να αναφέρεται σεDirectoryInfo εάν η καταχώρηση είναι κατάλογος.

### Παραδείγματα

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### Δείτε επίσης

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tararchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| fileInfo | FileInfo | Τα μεταδεδομένα του αρχείου ή του φακέλου που πρόκειται να συμπιεστούν. |
| openImmediately | Boolean | Σωστό εάν ανοίξετε το αρχείο αμέσως, διαφορετικά ανοίξτε το αρχείο κατά την αποθήκευση αρχειοθέτησης. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής πίσσας.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| PathTooLongException | *name* είναι πολύ μεγάλη για την πίσσα από το πρότυπο IEEE 1003.1-1998. |
| ArgumentException | Όνομα αρχείου, ως μέρος του*name*, υπερβαίνει τα 100 σύμβολα. |

### Παρατηρήσεις

Το όνομα καταχώρισης ορίζεται αποκλειστικά μέσα*name* παράμετρος. Το όνομα αρχείου που παρέχεται*fileInfo* η παράμετρος δεν επηρεάζει το όνομα της καταχώρισης.

*fileInfo* μπορεί να αναφέρεται σεDirectoryInfo εάν η καταχώρηση είναι κατάλογος.

Εάν το αρχείο ανοίξει αμέσως με*openImmediately*η παράμετρος αποκλείεται μέχρι να διατεθεί το αρχείο.

### Παραδείγματα

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### Δείτε επίσης

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tararchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| path | String | Διαδρομή προς το αρχείο που θα συμπιεστεί. |
| openImmediately | Boolean | Σωστό εάν ανοίξετε το αρχείο αμέσως, διαφορετικά ανοίξτε το αρχείο κατά την αποθήκευση αρχειοθέτησης. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής πίσσας.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *path* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*path* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. - ή - Όνομα αρχείου, ως μέρος του*name*, υπερβαίνει τα 100 σύμβολα. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*path* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*path* , όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. - ή -*name* είναι πολύ μεγάλη για την πίσσα από το πρότυπο IEEE 1003.1-1998. |
| NotSupportedException | Αρχείο στο*path* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |

### Παρατηρήσεις

Το όνομα καταχώρισης ορίζεται αποκλειστικά μέσα*name* παράμετρος. Το όνομα αρχείου που παρέχεται*path* η παράμετρος δεν επηρεάζει το όνομα της καταχώρισης.

Εάν το αρχείο ανοίξει αμέσως με*openImmediately*η παράμετρος αποκλείεται μέχρι να διατεθεί το αρχείο.

### Παραδείγματα

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### Δείτε επίσης

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tararchive/)
* συνέλευση [Aspose.Zip](../../../)


