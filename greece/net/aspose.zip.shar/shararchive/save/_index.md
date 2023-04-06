---
title: SharArchive.Save
second_title: Aspose.ZIP για Αναφορά API .NET
description: SharArchive μέθοδος. Αποθηκεύει το αρχείο στο παρεχόμενο αρχείο προορισμού.
type: docs
weight: 70
url: /el/net/aspose.zip.shar/shararchive/save/
---
## Save(string) {#save_1}

Αποθηκεύει το αρχείο στο παρεχόμενο αρχείο προορισμού.

```csharp
public void Save(string destinationFileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου παραπέμπει σε ένα υπάρχον αρχείο, θα αντικατασταθεί. |

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
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### Δείτε επίσης

* class [SharArchive](../)
* χώρος ονομάτων [Aspose.Zip.Shar](../../shararchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

Αποθηκεύει το αρχείο στη ροή που παρέχεται.

```csharp
public void Save(Stream output)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *output* είναι μηδενικό. |
| ArgumentException | *output* δεν είναι εγγράψιμο. - ή -*output* είναι το ίδιο ρεύμα από το οποίο εξάγουμε. |

### Παρατηρήσεις

*output*πρέπει να είναι εγγράψιμο.

### Παραδείγματα

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### Δείτε επίσης

* class [SharArchive](../)
* χώρος ονομάτων [Aspose.Zip.Shar](../../shararchive/)
* συνέλευση [Aspose.Zip](../../../)


