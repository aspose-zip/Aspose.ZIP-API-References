---
title: "CpioArchive.Save"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "CpioArchive μέθοδος. Αποθηκεύει το αρχείο σε ένα παρεχόμενο αρχείο προορισμού"
type: docs
weight: 80
url: /el/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

Αποθηκεύει το αρχείο σε προορισμένο αρχείο που παρέχεται.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| cpioFormat | CpioFormat | Ορίζει τη μορφή κεφαλίδας cpio. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *destinationFileName* είναι μια συμβολοσειρά μηδενικού μήκους, περιέχει μόνο κενά διαστήματα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες όπως ορίζονται από System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* είναι null. |
| PathTooLongException | Το καθορισμένο *destinationFileName*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες στα Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| DirectoryNotFoundException | Το καθορισμένο *destinationFileName* δεν είναι έγκυρο, (π.χ., βρίσκεται σε μη αντιστοιχισμένο δίσκο). |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά το άνοιγμα του αρχείου. |
| UnauthorizedAccessException | *destinationFileName* Καθορίζεται ένα αρχείο μόνο για ανάγνωση και η πρόσβαση δεν είναι ανάγνωση. -ή- η διαδρομή καθορίζεται ως φάκελος. -ή- ο καλών δεν έχει την απαιτούμενη άδεια. |
| NotSupportedException | *destinationFileName* βρίσκεται σε μη έγκυρη μορφή. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παρατηρήσεις

Είναι δυνατόν να αποθηκεύσετε ένα αρχείο στην ίδια διαδρομή από την οποία φορτώθηκε. Ωστόσο, αυτό δεν συνιστάται επειδή αυτή η προσέγγιση χρησιμοποιεί αντιγραφή σε προσωρινό αρχείο.

## Παραδείγματα

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### Δείτε επίσης

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |
| cpioFormat | CpioFormat | Ορίζει τη μορφή κεφαλίδας cpio. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *output* είναι null. |
| ArgumentException | *output* δεν είναι εγγράψιμο. -ή- *output* είναι η ίδια ροή από την οποία εξάγουμε. -Ή- Είναι αδύνατο να αποθηκευτεί το αρχείο σε *cpioFormat* λόγω περιορισμών μορφής. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παρατηρήσεις

*output* must be writable.

## Παραδείγματα

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(cpioFile);
    }
}       
```

### Δείτε επίσης

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


