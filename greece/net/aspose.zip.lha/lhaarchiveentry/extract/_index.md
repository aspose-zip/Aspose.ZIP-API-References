---
title: "LhaArchiveEntry.Extract"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος LhaArchiveEntry. Εξάγει την καταχώρηση του αρχείου Lha σε σύστημα αρχείων με βάση τη διαδρομή"
type: docs
weight: 60
url: /el/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

Εξάγει την καταχώρηση του αρχείου Lha σε σύστημα αρχείων με βάση τη διαδρομή.

```csharp
public FileSystemInfo Extract(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Διαδρομή προς το αρχείο που θα αποθηκεύσει τα αποσυμπιεσμένα δεδομένα. |

### Τιμή Επιστροφής

FileSystemInfoInstance που περιέχει τα εξαγόμενα δεδομένα.

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
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |
| InvalidDataException | Εκτοπίζεται όταν τα δεδομένα είναι μη έγκυρα ή κατεστραμμένα. |

## Παραδείγματα

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Δείτε επίσης

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

Εξάγει την καταχώρηση στη δοθείσα ροή.

```csharp
public void Extract(Stream destination)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | Stream | Ροή προορισμού. Πρέπει να είναι εγγράψιμη. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *destination* δεν υποστηρίζει εγγραφή. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |
| InvalidDataException | Εκτοπίζεται όταν τα δεδομένα είναι μη έγκυρα ή κατεστραμμένα. |

## Παρατηρήσεις

Δεν κάνει τίποτα για την καταχώρηση καταλόγου.

### Δείτε επίσης

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Εξάγει την καταχώρηση του αρχείου Lha σε ένα αρχείο.

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
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |

## Παρατηρήσεις

Δεν κάνει τίποτα για την καταχώρηση καταλόγου.

## Παραδείγματα

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Δείτε επίσης

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


