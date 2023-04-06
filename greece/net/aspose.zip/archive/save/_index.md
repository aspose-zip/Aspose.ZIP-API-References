---
title: Archive.Save
second_title: Aspose.ZIP για Αναφορά API .NET
description: Archive μέθοδος. Αποθηκεύει το αρχείο στη ροή που παρέχεται.
type: docs
weight: 90
url: /el/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

Αποθηκεύει το αρχείο στη ροή που παρέχεται.

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outputStream | Stream | Ροή προορισμού. |
| saveOptions | ArchiveSaveOptions | Επιλογές για αποθήκευση αρχείου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *outputStream* δεν είναι εγγράψιμο. |

### Παρατηρήσεις

*outputStream*πρέπει να είναι εγγράψιμο.

### Παραδείγματα

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(zipFile);
    }
}
```

### Δείτε επίσης

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

Αποθηκεύει το αρχείο στο παρεχόμενο αρχείο προορισμού.

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου παραπέμπει σε ένα υπάρχον αρχείο, θα αντικατασταθεί. |
| saveOptions | ArchiveSaveOptions | Επιλογές για αποθήκευση αρχείου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *destinationFileName* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*destinationFileName* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*destinationFileName* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*destinationFileName*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*destinationFileName* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |

### Παρατηρήσεις

Είναι δυνατό να αποθηκεύσετε ένα αρχείο στην ίδια διαδρομή από το οποίο φορτώθηκε. Ωστόσο, αυτό δεν συνιστάται επειδή αυτή η προσέγγιση χρησιμοποιεί αντιγραφή σε προσωρινό αρχείο.

### Παραδείγματα

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Δείτε επίσης

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)


