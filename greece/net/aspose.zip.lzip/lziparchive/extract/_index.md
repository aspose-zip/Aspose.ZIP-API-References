---
title: LzipArchive.Extract
second_title: Aspose.ZIP για Αναφορά API .NET
description: LzipArchive μέθοδος. Εξάγει το αρχείο lzip σε μια ροή.
type: docs
weight: 40
url: /el/net/aspose.zip.lzip/lziparchive/extract/
---
## Extract(Stream) {#extract_1}

Εξάγει το αρχείο lzip σε μια ροή.

```csharp
public void Extract(Stream destination)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destination | Stream | Ροή για αποθήκευση αποσυμπιεσμένων δεδομένων. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| InvalidOperationException | Οι κεφαλίδες αρχειοθέτησης και οι πληροφορίες υπηρεσίας δεν διαβάστηκαν. |
| InvalidDataException | Σφάλμα στα δεδομένα στην κεφαλίδα ή στο άθροισμα ελέγχου. |
| ArgumentNullException | Η ροή προορισμού είναι μηδενική. |
| ArgumentException | Η ροή προορισμού δεν υποστηρίζει εγγραφή. |

### Παραδείγματα

```csharp
using (FileStream sourceLzipFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new LzipArchive(sourceLzipFile))
        {
               archive.Extract(extractedFile);
           }
       }
}
```

### Δείτε επίσης

* class [LzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Lzip](../../lziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract}

Εξάγει το αρχείο lzip σε ένα αρχείο.

```csharp
public void Extract(FileInfo fileInfo)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo για αποθήκευση αποσυμπιεσμένων δεδομένων. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| InvalidOperationException | Οι κεφαλίδες αρχειοθέτησης και οι πληροφορίες υπηρεσίας δεν διαβάστηκαν. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια για να ανοίξει το*fileInfo*. |
| ArgumentException | Η διαδρομή αρχείου είναι κενή ή περιέχει μόνο λευκά κενά. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| UnauthorizedAccessException | Η διαδρομή προς το αρχείο είναι μόνο για ανάγνωση ή είναι κατάλογος. |
| ArgumentNullException | *fileInfo* είναι μηδενικό. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή δεν είναι έγκυρη, όπως είναι σε μη αντιστοιχισμένη μονάδα δίσκου. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |

### Παραδείγματα

```csharp
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(lzipFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Δείτε επίσης

* class [LzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Lzip](../../lziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Extract(string) {#extract_2}

Εξάγει το αρχείο lzip σε ένα αρχείο κατά διαδρομή.

```csharp
public void Extract(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Διαδρομή προς το αρχείο που θα αποθηκεύει αποσυμπιεσμένα δεδομένα. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| InvalidOperationException | Οι κεφαλίδες αρχειοθέτησης και οι πληροφορίες υπηρεσίας δεν διαβάστηκαν. |
| ArgumentNullException | *path* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*path* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*path* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*path*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*path* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |

### Παραδείγματα

```csharp
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Δείτε επίσης

* class [LzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Lzip](../../lziparchive/)
* συνέλευση [Aspose.Zip](../../../)


