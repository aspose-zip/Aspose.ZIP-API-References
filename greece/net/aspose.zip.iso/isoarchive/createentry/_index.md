---
title: "IsoArchive.CreateEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος IsoArchive. Προσθέτει ένα αρχείο στην εικόνα ISO"
type: docs
weight: 40
url: /el/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

Προσθέτει ένα αρχείο στην εικόνα ISO.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Διαδρομή του αρχείου στο ISO. |
| filePath | String | Διαδρομή του αρχείου. |

### Τιμή Επιστροφής

Η καταχώρηση ISO δημιουργήθηκε.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | Το *filePath* είναι null. |
| ArgumentException | Το *filePath* είναι κενό, περιέχει μόνο λευκούς χαρακτήρες ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *filePath* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο *filePath* υπερβαίνει το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *filePath* περιέχει άνω-κάτω τελεία (:) στη μέση της συμβολοσειράς. |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά το άνοιγμα του αρχείου. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη (για παράδειγμα, βρίσκεται σε μη αντιστοιχισμένο δίσκο). |
| FileNotFoundException | Το αρχείο που καθορίζεται στο *filePath* δεν βρέθηκε. |
| InvalidOperationException | Το αρχείο δεν βρίσκεται σε λειτουργία επεξεργασίας. |

### Δείτε επίσης

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Προσθέτει ένα αρχείο στην εικόνα ISO.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Διαδρομή του αρχείου στο ISO. |
| source | Stream | Ροή που περιέχει τα δεδομένα του αρχείου. |

### Τιμή Επιστροφής

Η καταχώρηση ISO δημιουργήθηκε.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentNullException | Εκτοπίζεται όταν ένα *name* ή *source* είναι null. |
| InvalidOperationException | Το αρχείο δεν βρίσκεται σε λειτουργία επεξεργασίας. |

### Δείτε επίσης

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

Προσθέτει ένα αρχείο στην εικόνα ISO.

```csharp
public IsoEntry CreateEntry(string name)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Διαδρομή του φακέλου στο ISO. |

### Τιμή Επιστροφής

Η καταχώρηση ISO δημιουργήθηκε.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | `name` είναι null ή κενό. |
| InvalidOperationException | Το αρχείο είναι ανοιχτό για εξαγωγή. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

### Δείτε επίσης

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


