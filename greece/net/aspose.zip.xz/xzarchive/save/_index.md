---
title: XzArchive.Save
second_title: Aspose.ZIP για Αναφορά API .NET
description: XzArchive μέθοδος. Αποθηκεύει το αρχείο xz στην παρεχόμενη ροή.
type: docs
weight: 40
url: /el/net/aspose.zip.xz/xzarchive/save/
---
## Save(Stream) {#save}

Αποθηκεύει το αρχείο xz στην παρεχόμενη ροή.

```csharp
public void Save(Stream output)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *output* δεν υποστηρίζει την αναζήτηση. |
| ArgumentNullException | *output* είναι μηδενικό. |

### Παρατηρήσεις

*output* πρέπει να είναι αναζητήσιμο.

### Παραδείγματα

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    using (var archive = new XzArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Δείτε επίσης

* class [XzArchive](../)
* χώρος ονομάτων [Aspose.Zip.Xz](../../xzarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Αποθηκεύει το αρχείο xz στο παρεχόμενο αρχείο προορισμού.

```csharp
public void Save(string destinationFileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου παραπέμπει σε ένα υπάρχον αρχείο, θα αντικατασταθεί. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *destinationFileName* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*destinationFileName* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*destinationFileName* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*destinationFileName*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*destinationFileName* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |

### Παραδείγματα

```csharp
using (var archive = new XzArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.xz");
}
```

### Δείτε επίσης

* class [XzArchive](../)
* χώρος ονομάτων [Aspose.Zip.Xz](../../xzarchive/)
* συνέλευση [Aspose.Zip](../../../)


