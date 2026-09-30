---
title: "ZstandardArchive.Extract"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος ZstandardArchive. Εξάγει το αρχείο στην παρεχόμενη ροή"
type: docs
weight: 30
url: /el/net/aspose.zip.zstandard/zstandardarchive/extract/
---
## Extract(Stream) {#extract_1}

Εξάγει το αρχείο στο παρεχόμενο ρεύμα.

```csharp
public void Extract(Stream destination)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | Stream | Ροή προορισμού. Πρέπει να είναι εγγράψιμη. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentException | *destination* δεν υποστηρίζει εγγραφή. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |

## Παραδείγματα

```csharp
using (var archive = new GzipArchive("archive.zst"))
{
     archive.Extract(httpResponseStream);
}
```

### Δείτε επίσης

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Εξάγει το αρχείο στο αρχείο με βάση τη διαδρομή.

```csharp
public FileInfo Extract(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί. |

### Τιμή Επιστροφής

Πληροφορίες ενός εξαγόμενου αρχείου.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |

### Δείτε επίσης

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


