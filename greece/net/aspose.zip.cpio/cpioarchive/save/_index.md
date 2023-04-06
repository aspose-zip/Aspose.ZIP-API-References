---
title: CpioArchive.Save
second_title: Aspose.ZIP για Αναφορά API .NET
description: CpioArchive μέθοδος. Αποθηκεύει το αρχείο στο παρεχόμενο αρχείο προορισμού.
type: docs
weight: 80
url: /el/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

Αποθηκεύει το αρχείο στο παρεχόμενο αρχείο προορισμού.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου παραπέμπει σε ένα υπάρχον αρχείο, θα αντικατασταθεί. |
| cpioFormat | CpioFormat | Καθορίζει τη μορφή κεφαλίδας cpio. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *destinationFileName* είναι μια συμβολοσειρά μηδενικού μήκους, περιέχει μόνο λευκό διάστημα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες όπως ορίζονται από το System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* είναι μηδενικό. |
| PathTooLongException | Το καθορισμένο*destinationFileName*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| DirectoryNotFoundException | Το καθορισμένο*destinationFileName* δεν είναι έγκυρο, (για παράδειγμα, βρίσκεται σε μη αντιστοιχισμένη μονάδα δίσκου). |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά το άνοιγμα του αρχείου. |
| UnauthorizedAccessException | *destinationFileName* καθόρισε ένα αρχείο που είναι μόνο για ανάγνωση και η πρόσβαση δεν είναι Ανάγνωση.-ή- η διαδρομή καθόρισε έναν κατάλογο.-ή- Ο καλών δεν έχει την απαιτούμενη άδεια. |
| NotSupportedException | *destinationFileName* είναι σε μη έγκυρη μορφή. |

### Παρατηρήσεις

Είναι δυνατό να αποθηκεύσετε ένα αρχείο στην ίδια διαδρομή από το οποίο φορτώθηκε. Ωστόσο, αυτό δεν συνιστάται επειδή αυτή η προσέγγιση χρησιμοποιεί αντιγραφή σε προσωρινό αρχείο.

### Παραδείγματα

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
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

Αποθηκεύει το αρχείο στη ροή που παρέχεται.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |
| cpioFormat | CpioFormat | Καθορίζει τη μορφή κεφαλίδας cpio. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *output* είναι μηδενικό. |
| ArgumentException | *output* δεν είναι εγγράψιμο. - ή -*output* είναι η ίδια ροή από την οποία εξάγουμε. - Ή - Είναι αδύνατη η αποθήκευση του αρχείου σε*cpioFormat* λόγω περιορισμών μορφής. |

### Παρατηρήσεις

*output*πρέπει να είναι εγγράψιμο.

### Παραδείγματα

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
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)


