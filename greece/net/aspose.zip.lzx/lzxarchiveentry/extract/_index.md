---
title: "LzxArchiveEntry.Extract"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "LzxArchiveEntry μέθοδος. Εξάγει την καταχώρηση του αρχείου Lzx σε σύστημα αρχείων με βάση τη διαδρομή."
type: docs
weight: 80
url: /el/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

Εξάγει την καταχώρηση του αρχείου Lzx σε σύστημα αρχείων με βάση τη διαδρομή.

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
| InvalidDataException | Ασυμφωνία αθροίσματος ελέγχου για κεφαλίδες ή δεδομένα. - ή - Το αρχείο είναι κατεστραμμένο. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |
| NotSupportedException | Μη έγκυρη μέθοδος συμπίεσης. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |
| EndOfStreamException | Εκτοπίζεται όταν το τέλος της ροής επιτυγχάνεται απροσδόκητα. |

## Παραδείγματα

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Δείτε επίσης

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

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
| InvalidDataException | Ασυμφωνία αθροίσματος ελέγχου για κεφαλίδες ή δεδομένα. - ή - Το αρχείο είναι κατεστραμμένο. |
| ArgumentNullException | Η ροή προορισμού είναι null. |
| NotSupportedException | Μη έγκυρη μέθοδος συμπίεσης. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |
| EndOfStreamException | Εκτοπίζεται όταν το τέλος της ροής επιτυγχάνεται απροσδόκητα. |

### Δείτε επίσης

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


