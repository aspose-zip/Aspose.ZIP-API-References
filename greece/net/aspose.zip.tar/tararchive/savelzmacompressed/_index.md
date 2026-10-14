---
title: "TarArchive.SaveLZMACompressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος TarArchive. Αποθηκεύει το αρχείο στη ροή με συμπίεση LZMA"
type: docs
weight: 190
url: /el/net/aspose.zip.tar/tararchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, TarFormat?) {#savelzmacompressed}

Αποθηκεύει το αρχείο στη ροή με συμπίεση LZMA.

```csharp
public void SaveLZMACompressed(Stream output, TarFormat? format = default)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |
| μορφή | Nullable`1 | Ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *output* είναι null. |
| ArgumentException | *output* δεν είναι εγγράψιμο. |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί και δεν μπορεί να χρησιμοποιηθεί |
| IOException | Παρουσιάστηκε σφάλμα I/O. |

## Παρατηρήσεις

*output* must be writable.

Σημαντικό: το αρχείο tar δημιουργείται και στη συνέχεια συμπιέζεται μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

## Παραδείγματα

```csharp
using (FileStream result = File.OpenWrite("result.tar.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### Δείτε επίσης

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZMACompressed(string, TarFormat?) {#savelzmacompressed_1}

Αποθηκεύει το αρχείο στο αρχείο μέσω διαδρομής με συμπίεση lzma.

```csharp
public void SaveLZMACompressed(string path, TarFormat? format = default)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| μορφή | Nullable`1 | Ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| UnauthorizedAccessException | Ο καλών δεν διαθέτει την απαιτούμενη άδεια. -ή- *path* καθόρισε ένα αρχείο ή φάκελο μόνο για ανάγνωση. |
| ArgumentException | *path* είναι συμβολοσειρά μηδενικού μήκους, περιέχει μόνο κενά ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες όπως ορίζονται από InvalidPathChars. |
| ArgumentNullException | *path* είναι null. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| DirectoryNotFoundException | Το καθορισμένο *path* είναι μη έγκυρο, (π.χ., βρίσκεται σε μη αντιστοιχισμένο δίσκο). |
| NotSupportedException | *path* έχει μη έγκυρη μορφή. |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί και δεν μπορεί να χρησιμοποιηθεί |
| IOException | Παρουσιάστηκε σφάλμα I/O. |

## Παρατηρήσεις

Σημαντικό: το αρχείο tar δημιουργείται και στη συνέχεια συμπιέζεται μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

## Παραδείγματα

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.tar.lzma");
    }
}
```

### Δείτε επίσης

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


