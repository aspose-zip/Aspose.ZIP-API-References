---
title: ZArchive.Save
second_title: Aspose.ZIP για Αναφορά API .NET
description: ZArchive μέθοδος. Αποθηκεύει το αρχείο xz στην παρεχόμενη ροή.
type: docs
weight: 40
url: /el/net/aspose.zip.z/zarchive/save/
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
using (FileStream zFile = File.Open("data.bin.z", FileMode.Create))
{
    using (var archive = new ZArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(zFile);
     }
}
```

### Δείτε επίσης

* class [ZArchive](../)
* χώρος ονομάτων [Aspose.Zip.Z](../../zarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Αποθηκεύει το αρχείο Z στο παρεχόμενο αρχείο προορισμού.

```csharp
public void Save(string destinationFileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | +Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου παραπέμπει σε ένα υπάρχον αρχείο, θα αντικατασταθεί. |

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
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### Δείτε επίσης

* class [ZArchive](../)
* χώρος ονομάτων [Aspose.Zip.Z](../../zarchive/)
* συνέλευση [Aspose.Zip](../../../)


