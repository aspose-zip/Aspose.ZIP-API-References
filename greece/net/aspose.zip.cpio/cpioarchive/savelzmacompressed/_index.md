---
title: "CpioArchive.SaveLZMACompressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος CpioArchive. Αποθηκεύει το αρχείο στην ροή με συμπίεση LZMA."
type: docs
weight: 110
url: /el/net/aspose.zip.cpio/cpioarchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, CpioFormat) {#savelzmacompressed}

Αποθηκεύει το αρχείο στη ροή με συμπίεση LZMA.

```csharp
public void SaveLZMACompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |
| cpioFormat | CpioFormat | Ορίζει τη μορφή κεφαλίδας cpio. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| NotSupportedException | Η ροή δεν υποστηρίζει εγγραφή, ή η ροή είναι ήδη κλειστή. |

## Παρατηρήσεις

*output* must be writable.

Σημαντικό: το αρχείο cpio δημιουργείται και στη συνέχεια συμπιέζεται μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

## Παραδείγματα

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### Δείτε επίσης

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZMACompressed(string, CpioFormat) {#savelzmacompressed_1}

Αποθηκεύει το αρχείο στο αρχείο μέσω διαδρομής με συμπίεση lzma.

```csharp
public void SaveLZMACompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| cpioFormat | CpioFormat | Ορίζει τη μορφή κεφαλίδας cpio. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentNullException | *path* είναι `null`. |
| Εξαίρεση | Εκτοξεύεται όταν συμβαίνει σφάλμα χρόνου εκτέλεσης. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη (για παράδειγμα, βρίσκεται σε μη αντιστοιχισμένο δίσκο). |
| IOException | Παρουσιάστηκε σφάλμα I/O. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. |
| UnauthorizedAccessException | Ο καλών δεν διαθέτει την απαιτούμενη άδεια. -ή- *path* καθόρισε ένα αρχείο ή φάκελο μόνο για ανάγνωση. |

## Παρατηρήσεις

Σημαντικό: το αρχείο cpio δημιουργείται και στη συνέχεια συμπιέζεται μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

## Παραδείγματα

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.cpio.lzma");
    }
}
```

### Δείτε επίσης

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


