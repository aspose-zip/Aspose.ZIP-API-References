---
title: ArchiveEntry.Extract
second_title: Aspose.ZIP για Αναφορά API .NET
description: ArchiveEntry μέθοδος. Εξάγει την καταχώρηση στο σύστημα αρχείων από τη διαδρομή που παρέχεται.
type: docs
weight: 100
url: /el/net/aspose.zip/archiveentry/extract/
---
## Extract(string, string) {#extract}

Εξάγει την καταχώρηση στο σύστημα αρχείων από τη διαδρομή που παρέχεται.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί. |
| password | String | Προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση. |

### Επιστρεφόμενη Αξία

Οι πληροφορίες αρχείου του σύνθετου αρχείου.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *path* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*path* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*path* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*path*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*path* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |
| InvalidDataException | Η επαλήθευση CRC ή MAC απέτυχε για την καταχώριση. |

### Παραδείγματα

Εξαγάγετε δύο καταχωρήσεις του αρχείου zip, η καθεμία με τον δικό της κωδικό πρόσβασης

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
* χώρος ονομάτων [Aspose.Zip](../../archiveentry/)
* συνέλευση [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Εξάγει την καταχώρηση στη ροή που παρέχεται.

```csharp
public void Extract(Stream destination, string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destination | Stream | Ροή προορισμού. Πρέπει να είναι εγγράψιμο. |
| password | String | Προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| InvalidDataException | Η επαλήθευση CRC ή MAC απέτυχε για την καταχώριση. |
| ArgumentException | *destination* δεν υποστηρίζει τη γραφή. |

### Παραδείγματα

Εξαγωγή μιας καταχώρησης αρχείου zip με κωδικό πρόσβασης.

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
* χώρος ονομάτων [Aspose.Zip](../../archiveentry/)
* συνέλευση [Aspose.Zip](../../../)


