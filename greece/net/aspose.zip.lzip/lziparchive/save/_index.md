---
title: LzipArchive.Save
second_title: Aspose.ZIP για Αναφορά API .NET
description: LzipArchive μέθοδος. Αποθηκεύει το αρχείο lzip στη ροή που παρέχεται.
type: docs
weight: 50
url: /el/net/aspose.zip.lzip/lziparchive/save/
---
## Save(Stream) {#save_1}

Αποθηκεύει το αρχείο lzip στη ροή που παρέχεται.

```csharp
public void Save(Stream outputStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outputStream | Stream | Ροή προορισμού. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *outputStream* δεν υποστηρίζει την αναζήτηση. |
| ArgumentNullException | *outputStream* είναι μηδενικό. |

### Παρατηρήσεις

*outputStream* πρέπει να είναι αναζητήσιμο.

### Παραδείγματα

```csharp
using (FileStream lzFile = File.Open("archive.lz", FileMode.Create))
{
    using (var archive = new LzipArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzFile);
     }
}
```

### Δείτε επίσης

* class [LzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Lzip](../../lziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Αποθηκεύει το αρχείο lzip στο παρεχόμενο αρχείο προορισμού.

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
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lz");
}
```

### Δείτε επίσης

* class [LzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Lzip](../../lziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Αποθηκεύει το αρχείο lzip στο παρεχόμενο αρχείο προορισμού.

```csharp
public void Save(FileInfo destination)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destination | FileInfo | FileInfo που θα ανοίξει ως ροή προορισμού. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια για να ανοίξει το*destination*. |
| ArgumentException | Η διαδρομή αρχείου είναι κενή ή περιέχει μόνο λευκά κενά. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| UnauthorizedAccessException | Η διαδρομή προς το αρχείο είναι μόνο για ανάγνωση ή είναι κατάλογος. |
| ArgumentNullException | *destination* είναι μηδενικό. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή δεν είναι έγκυρη, όπως είναι σε μη αντιστοιχισμένη μονάδα δίσκου. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |

### Παραδείγματα

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz"));
}
```

### Δείτε επίσης

* class [LzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Lzip](../../lziparchive/)
* συνέλευση [Aspose.Zip](../../../)


