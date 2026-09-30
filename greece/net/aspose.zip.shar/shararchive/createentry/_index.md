---
title: "SharArchive.CreateEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος SharArchive. Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο."
type: docs
weight: 40
url: /el/net/aspose.zip.shar/shararchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public SharEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| fileInfo | FileInfo | Τα μεταδεδομένα του αρχείου ή φακέλου που θα συμπιεστεί. |
| openImmediately | Boolean | True, εάν το αρχείο ανοίξει αμέσως, διαφορετικά το αρχείο ανοίγει κατά την αποθήκευση του αρχείου. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Shar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *name* είναι null. |
| ArgumentException | *name* είναι κενό. |
| ArgumentNullException | *fileInfo* είναι null. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Το αρχείο του είναι ανοιχτό για εξαγωγή. |

## Παρατηρήσεις

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο *openImmediately*, θα παραμείνει κλειδωμένο μέχρι να απελευθερωθεί το αρχείο.

## Παραδείγματα

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new SharArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.shar");
}
```

### Δείτε επίσης

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public SharEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| sourcePath | String | Διαδρομή προς το αρχείο που θα συμπιεστεί. |
| openImmediately | Boolean | True, εάν το αρχείο ανοίξει αμέσως, διαφορετικά το αρχείο ανοίγει κατά την αποθήκευση του αρχείου. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Shar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *sourcePath* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Το *sourcePath* είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει άκυρους χαρακτήρες. - ή - Το όνομα αρχείου, ως μέρος του *name*, υπερβαίνει τα 100 σύμβολα. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *sourcePath* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο *sourcePath*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. - ή - *name* είναι πολύ μακρύ για το shar. |
| NotSupportedException | Το αρχείο στο *sourcePath* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Αυτό το αρχείο είναι ανοιχτό για εξαγωγή. |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά από την παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *sourcePath* δεν επηρεάζει το όνομα της καταχώρησης.

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο *openImmediately*, θα παραμείνει κλειδωμένο μέχρι να απελευθερωθεί το αρχείο.

## Παραδείγματα

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Δείτε επίσης

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public SharEntry CreateEntry(string name, Stream source)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Shar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *name* είναι null. |
| ArgumentNullException | *source* είναι null. |
| ArgumentException | *name* είναι κενό. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Αυτό το αρχείο είναι ανοιχτό για εξαγωγή. |

## Παραδείγματα

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.shar");
}
```

### Δείτε επίσης

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


