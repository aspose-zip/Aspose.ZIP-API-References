---
title: "TarArchive.CreateEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος TarArchive. Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο"
type: docs
weight: 110
url: /el/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |
| fileInfo | FileSystemInfo | Τα μεταδεδομένα του αρχείου ή φακέλου που θα συμπιεστεί. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Tar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| PathTooLongException | *name* είναι πολύ μεγάλο για tar σύμφωνα με το πρότυπο IEEE 1003.1-1998. |
| ArgumentException | Το όνομα αρχείου, ως μέρος του *name*, υπερβαίνει τα 100 σύμβολα. |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί και δεν μπορεί να χρησιμοποιηθεί |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *fileInfo* δεν επηρεάζει το όνομα της καταχώρησης.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## Παραδείγματα

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
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| fileInfo | FileInfo | Τα μεταδεδομένα του αρχείου ή φακέλου που θα συμπιεστεί. |
| openImmediately | Boolean | True, εάν το αρχείο ανοίξει αμέσως, διαφορετικά το αρχείο ανοίγει κατά την αποθήκευση του αρχείου. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Tar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| PathTooLongException | *name* είναι πολύ μεγάλο για tar σύμφωνα με το πρότυπο IEEE 1003.1-1998. |
| ArgumentException | Το όνομα αρχείου, ως μέρος του *name*, υπερβαίνει τα 100 σύμβολα. |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί και δεν μπορεί να χρησιμοποιηθεί |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *fileInfo* δεν επηρεάζει το όνομα της καταχώρησης.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο *openImmediately*, θα παραμείνει κλειδωμένο μέχρι να απελευθερωθεί το αρχείο.

## Παραδείγματα

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
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| διαδρομή | String | Διαδρομή προς το αρχείο που θα συμπιεστεί. |
| openImmediately | Boolean | True, εάν το αρχείο ανοίξει αμέσως, διαφορετικά το αρχείο ανοίγει κατά την αποθήκευση του αρχείου. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Tar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Το *path* είναι κενό, περιέχει μόνο κενά ή περιέχει μη έγκυρους χαρακτήρες. - ή - Το όνομα αρχείου, ως μέρος του *name*, υπερβαίνει τα 100 σύμβολα. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες Windows, τα μονοπάτια πρέπει να είναι μικρότερα από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. - ή - *name* είναι πολύ μεγάλο για tar σύμφωνα με το πρότυπο IEEE 1003.1-1998. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί και δεν μπορεί να χρησιμοποιηθεί |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *path* δεν επηρεάζει το όνομα της καταχώρησης.

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο *openImmediately*, θα παραμείνει κλειδωμένο μέχρι να απελευθερωθεί το αρχείο.

## Παραδείγματα

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
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


