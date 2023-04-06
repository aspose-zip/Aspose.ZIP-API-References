---
title: CpioArchive.CreateEntry
second_title: Aspose.ZIP για Αναφορά API .NET
description: CpioArchive μέθοδος. Δημιουργία μίας καταχώρησης μέσα στο αρχείο.
type: docs
weight: 40
url: /el/net/aspose.zip.cpio/cpioarchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public CpioEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| fileInfo | FileInfo | Τα μεταδεδομένα του αρχείου ή του φακέλου που πρόκειται να συμπιεστούν. |
| openImmediately | Boolean | Σωστό εάν ανοίξετε το αρχείο αμέσως, διαφορετικά ανοίξτε το αρχείο κατά την αποθήκευση αρχειοθέτησης. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής Cpio.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *name* είναι μηδενικό. |
| ArgumentException | *name* είναι άδειο. |
| ArgumentNullException | *fileInfo* είναι μηδενικό. |

### Παρατηρήσεις

Εάν το αρχείο ανοίξει αμέσως με*openImmediately*η παράμετρος αποκλείεται μέχρι να διατεθεί το αρχείο.

### Παραδείγματα

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new CpioArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.cpio");
}
```

### Δείτε επίσης

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public CpioEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| sourcePath | String | Διαδρομή προς το αρχείο που θα συμπιεστεί. |
| openImmediately | Boolean | Σωστό εάν ανοίξετε το αρχείο αμέσως, διαφορετικά ανοίξτε το αρχείο κατά την αποθήκευση αρχειοθέτησης. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής Cpio.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *sourcePath* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*sourcePath* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. - ή - Όνομα αρχείου, ως μέρος του*name*, υπερβαίνει τα 100 σύμβολα. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*sourcePath* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*sourcePath* , όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. - ή -*name* είναι πολύ μεγάλο για cpio. |
| NotSupportedException | Αρχείο στο*sourcePath* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |

### Παρατηρήσεις

Το όνομα καταχώρισης ορίζεται αποκλειστικά μέσα*name* παράμετρος. Το όνομα αρχείου που παρέχεται*sourcePath* η παράμετρος δεν επηρεάζει το όνομα της καταχώρισης.

Εάν το αρχείο ανοίξει αμέσως με*openImmediately*η παράμετρος αποκλείεται μέχρι να διατεθεί το αρχείο.

### Παραδείγματα

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Δείτε επίσης

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public CpioEntry CreateEntry(string name, Stream source)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής Cpio.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *name* είναι μηδενικό. |
| ArgumentNullException | *source* είναι μηδενικό. |
| ArgumentException | *name* είναι άδειο. |

### Παραδείγματα

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.cpio");
}
```

### Δείτε επίσης

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)


