---
title: "SnappyArchive.Extract"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος SnappyArchive. Εξάγει το snappy archive σε μια ροή."
type: docs
weight: 30
url: /el/net/aspose.zip.snappy/snappyarchive/extract/
---
## Extract(Stream) {#extract_2}

Εξάγει το αρχείο snappy σε ροή.

```csharp
public void Extract(Stream destination)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | Stream | Ροή για την αποθήκευση αποσυμπιεσμένων δεδομένων. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Οι κεφαλίδες του αρχείου και οι πληροφορίες υπηρεσίας δεν διαβάστηκαν. |
| InvalidDataException | Σφάλμα στα δεδομένα στην κεφαλίδα ή στο checksum. |
| ArgumentNullException | Η ροή προορισμού είναι null. |
| ArgumentException | Η ροή προορισμού δεν υποστηρίζει εγγραφή. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

```csharp
using (FileStream sourceSnappyFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
   {
       using (var archive = new SnappyArchive(sourceSnappyFile))
       {
           archive.Extract(extractedFile);
       }
   }
}
```

### Δείτε επίσης

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Εξάγει το αρχείο snappy σε αρχείο.

```csharp
public void Extract(FileInfo fileInfo)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo για αποθήκευση αποσυμπιεσμένων δεδομένων. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Οι κεφαλίδες του αρχείου και οι πληροφορίες υπηρεσίας δεν διαβάστηκαν. |
| SecurityException | Το πρόγραμμα που καλεί δεν έχει την απαιτούμενη άδεια για το άνοιγμα του *fileInfo*. |
| ArgumentException | Η διαδρομή του αρχείου είναι κενή ή περιέχει μόνο κενά διαστήματα. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| UnauthorizedAccessException | Η διαδρομή προς το αρχείο είναι μόνο για ανάγνωση ή είναι κατάλογος. |
| ArgumentNullException | *fileInfo* είναι null. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

```csharp
using (FileStream snappyFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new SnappyArchive(snappyFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Δείτε επίσης

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Εξάγει το αρχείο snappy σε αρχείο με βάση τη διαδρομή.

```csharp
public FileInfo Extract(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Διαδρομή προς το αρχείο που θα αποθηκεύσει τα αποσυμπιεσμένα δεδομένα. |

### Τιμή Επιστροφής

Παράδειγμα FileInfo που περιέχει τα εξαγόμενα δεδομένα.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Οι κεφαλίδες του αρχείου και οι πληροφορίες υπηρεσίας δεν διαβάστηκαν. |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |

## Παραδείγματα

```csharp
using (FileStream snappyFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new SnappyArchive(snappyFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Δείτε επίσης

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)


