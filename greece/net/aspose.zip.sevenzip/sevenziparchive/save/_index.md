---
title: SevenZipArchive.Save
second_title: Aspose.ZIP για Αναφορά API .NET
description: SevenZipArchive μέθοδος. Αποθηκεύει το αρχείο 7z στην παρεχόμενη ροή.
type: docs
weight: 80
url: /el/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

Αποθηκεύει το αρχείο 7z στην παρεχόμενη ροή.

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
| InvalidOperationException | Ο κωδικοποιητής απέτυχε να συμπιέσει τα δεδομένα. |

### Παρατηρήσεις

*output* πρέπει να είναι αναζητήσιμο.

### Παραδείγματα

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### Δείτε επίσης

* class [SevenZipArchive](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)

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
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### Δείτε επίσης

* class [SevenZipArchive](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)


