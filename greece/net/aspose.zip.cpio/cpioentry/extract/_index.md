---
title: "CpioEntry.Extract"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος CpioEntry. Εξάγει την καταχώρηση στο σύστημα αρχείων με τη δοθείσα διαδρομή"
type: docs
weight: 60
url: /el/net/aspose.zip.cpio/cpioentry/extract/
---
## Extract(string) {#extract}

Εξάγει την καταχώρηση στο σύστημα αρχείων με τη δοθείσα διαδρομή.

```csharp
public FileSystemInfo Extract(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί. |

### Τιμή Επιστροφής

Οι πληροφορίες αρχείου ενός σύνθετου αρχείου.

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
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |

## Παραδείγματα

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Δείτε επίσης

* class [CpioEntry](../)
* namespace [Aspose.Zip.Cpio](../../cpioentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Εξάγει την καταχώρηση στη δοθείσα ροή.

```csharp
public void Extract(Stream destination)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | Stream | Ροή προορισμού. Πρέπει να είναι εγγράψιμη. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *destination* δεν υποστηρίζει εγγραφή. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |

## Παραδείγματα

Εξάγετε μια καταχώρηση από το αρχείο cpio.

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Δείτε επίσης

* class [CpioEntry](../)
* namespace [Aspose.Zip.Cpio](../../cpioentry/)
* assembly [Aspose.Zip](../../../)


