---
title: "ArchiveEntry.Extract"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος ArchiveEntry. Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται"
type: docs
weight: 110
url: /el/net/aspose.zip/archiveentry/extract/
---
## Extract(string, string) {#extract}

Εξάγει την καταχώρηση στο σύστημα αρχείων με τη δοθείσα διαδρομή.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί. |
| password | String | Προαιρετικό password για αποκρυπτογράφηση. |

### Τιμή Επιστροφής

Οι πληροφορίες του συντιθέμενου αρχείου.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |
| InvalidDataException | Τα δεδομένα είναι κατεστραμμένα. -ή- Η επαλήθευση CRC ή MAC απέτυχε για την καταχώρηση. |
| ObjectDisposedException | Εκτοπίζεται εάν το αρχείο έχει διαγραφεί. |

## Παραδείγματα

Εξάγετε δύο καταχωρήσεις του αρχείου ZIP, η κάθε μία με τον δικό της κωδικό πρόσβασης

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract("first.bin", "first_pass");
        archive.Entries[1].Extract("second.bin", "second_pass");
    }
}
```

### Δείτε επίσης

* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Εξάγει την καταχώρηση στη δοθείσα ροή.

```csharp
public void Extract(Stream destination, string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | Stream | Ροή προορισμού. Πρέπει να είναι εγγράψιμη. |
| password | String | Προαιρετικό password για αποκρυπτογράφηση. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidDataException | Τα δεδομένα είναι κατεστραμμένα. -ή- Η επαλήθευση CRC ή MAC απέτυχε για την καταχώρηση. |
| IOException | Η πηγή είναι κατεστραμμένη ή μη αναγνώσιμη. |
| ArgumentException | *destination* δεν υποστηρίζει εγγραφή. |
| ObjectDisposedException | Εκτοπίζεται εάν το αρχείο έχει διαγραφεί. |

## Παραδείγματα

Εξάγετε μια καταχώρηση του αρχείου zip με κωδικό πρόσβασης.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### Δείτε επίσης

* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


