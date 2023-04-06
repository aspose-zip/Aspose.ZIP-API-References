---
title: ZArchive.Extract
second_title: Aspose.ZIP για Αναφορά API .NET
description: ZArchive μέθοδος. Εξάγει το αρχείο Z σε μια ροή.
type: docs
weight: 30
url: /el/net/aspose.zip.z/zarchive/extract/
---
## Extract(Stream) {#extract_2}

Εξάγει το αρχείο Z σε μια ροή.

```csharp
public void Extract(Stream destination)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destination | Stream | Ροή για αποθήκευση αποσυμπιεσμένων δεδομένων. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| InvalidDataException | Τα δεδομένα δεν μπορούν να αποσυμπιεστούν. |

### Παραδείγματα

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new ZArchive(zFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### Δείτε επίσης

* class [ZArchive](../)
* χώρος ονομάτων [Aspose.Zip.Z](../../zarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Εξάγει το αρχείο Z σε ένα αρχείο.

```csharp
public void Extract(FileInfo fileInfo)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo για αποθήκευση αποσυμπιεσμένων δεδομένων. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια για να ανοίξει το*fileInfo*. |
| ArgumentException | Η διαδρομή αρχείου είναι κενή ή περιέχει μόνο λευκά κενά. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| UnauthorizedAccessException | Η διαδρομή προς το αρχείο είναι μόνο για ανάγνωση ή είναι κατάλογος. |
| ArgumentNullException | *fileInfo* είναι μηδενικό. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή δεν είναι έγκυρη, όπως είναι σε μη αντιστοιχισμένη μονάδα δίσκου. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |
| InvalidDataException | Τα δεδομένα δεν μπορούν να αποσυμπιεστούν. |

### Παραδείγματα

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Δείτε επίσης

* class [ZArchive](../)
* χώρος ονομάτων [Aspose.Zip.Z](../../zarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Εξάγει το αρχείο Z σε ένα αρχείο κατά διαδρομή.

```csharp
public FileInfo Extract(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Διαδρομή προς το αρχείο που θα αποθηκεύει αποσυμπιεσμένα δεδομένα. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *path* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*path* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*path* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*path*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*path* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |
| InvalidDataException | Τα δεδομένα δεν μπορούν να αποσυμπιεστούν. |

### Παραδείγματα

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Δείτε επίσης

* class [ZArchive](../)
* χώρος ονομάτων [Aspose.Zip.Z](../../zarchive/)
* συνέλευση [Aspose.Zip](../../../)


