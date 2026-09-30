---
title: "LzipArchive.Extract"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "LzipArchive μέθοδος. Εξάγει το lzip αρχείο σε μια ροή"
type: docs
weight: 50
url: /el/net/aspose.zip.lzip/lziparchive/extract/
---
## Extract(Stream) {#extract_1}

Εξάγει το αρχείο lzip σε μια ροή.

```csharp
public void Extract(Stream destination)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | Stream | Ροή για την αποθήκευση αποσυμπιεσμένων δεδομένων. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Οι κεφαλίδες του αρχείου και οι πληροφορίες υπηρεσίας δεν διαβάστηκαν. |
| InvalidDataException | Σφάλμα στα δεδομένα στην κεφαλίδα ή στο checksum. |
| ArgumentNullException | Η ροή προορισμού είναι null. |
| ArgumentException | Η ροή προορισμού δεν υποστηρίζει εγγραφή. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |

## Παραδείγματα

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
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

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

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Οι κεφαλίδες του αρχείου και οι πληροφορίες υπηρεσίας δεν διαβάστηκαν. |
| SecurityException | Το πρόγραμμα που καλεί δεν έχει την απαιτούμενη άδεια για το άνοιγμα του *fileInfo*. |
| ArgumentException | Η διαδρομή του αρχείου είναι κενή ή περιέχει μόνο κενά διαστήματα. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| UnauthorizedAccessException | Η διαδρομή προς το αρχείο είναι μόνο για ανάγνωση ή είναι κατάλογος. |
| ArgumentNullException | *fileInfo* είναι null. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |

## Παραδείγματα

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
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract_2}

Εξάγει το αρχείο lzip σε αρχείο με βάση τη διαδρομή.

```csharp
public void Extract(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Διαδρομή προς το αρχείο που θα αποθηκεύσει τα αποσυμπιεσμένα δεδομένα. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Οι κεφαλίδες του αρχείου και οι πληροφορίες υπηρεσίας δεν διαβάστηκαν. |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |

## Παραδείγματα

```csharp
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(lzipFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Δείτε επίσης

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)


