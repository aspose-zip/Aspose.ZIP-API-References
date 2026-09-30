---
title: "CpioArchive.SaveZstandard"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος CpioArchive. Αποθηκεύει το αρχείο στην ροή με συμπίεση Zstandard"
type: docs
weight: 140
url: /el/net/aspose.zip.cpio/cpioarchive/savezstandard/
---
## SaveZstandard(Stream, CpioFormat) {#savezstandard}

Αποθηκεύει το αρχείο στο ρεύμα με συμπίεση Zstandard.

```csharp
public void SaveZstandard(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |
| cpioFormat | CpioFormat | Ορίζει τη μορφή κεφαλίδας cpio. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *output* είναι null. |
| ArgumentException | *output* δεν είναι εγγράψιμο. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παρατηρήσεις

*output* must be writable.

## Παραδείγματα

```csharp
using (FileStream result = File.OpenWrite("result.cpio.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
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

## SaveZstandard(string, CpioFormat) {#savezstandard_1}

Αποθηκεύει το αρχείο στο αρχείο μέσω διαδρομής με συμπίεση Zstandard.

```csharp
public void SaveZstandard(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| cpioFormat | CpioFormat | Ορίζει τη μορφή κεφαλίδας cpio. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentException | *path* είναι συμβολοσειρά μηδενικού μήκους, περιέχει μόνο κενά ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες όπως ορίζονται από InvalidPathChars. |
| ArgumentNullException | *path* είναι `null`. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη (για παράδειγμα, βρίσκεται σε μη αντιστοιχισμένο δίσκο). |
| IOException | Παρουσιάστηκε σφάλμα I/O. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. |
| UnauthorizedAccessException | Ο καλών δεν διαθέτει την απαιτούμενη άδεια. -ή- *path* καθόρισε ένα αρχείο ή φάκελο μόνο για ανάγνωση. |

## Παραδείγματα

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.cpio.zst");
    }
}
```

### Δείτε επίσης

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


