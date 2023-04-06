---
title: SevenZipArchiveEntry.Extract
second_title: Aspose.ZIP για Αναφορά API .NET
description: SevenZipArchiveEntry μέθοδος. Εξάγει την καταχώρηση στο σύστημα αρχείων από τη διαδρομή που παρέχεται.
type: docs
weight: 80
url: /el/net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
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

### Παραδείγματα

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Δείτε επίσης

* class [SevenZipArchiveEntry](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
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
| ArgumentException | *destination* δεν υποστηρίζει τη γραφή. |
| InvalidOperationException | Το αρχείο δεν ανοίγει για εξαγωγή. - ή - Αυτή η καταχώρηση είναι ένας κατάλογος. |
| InvalidDataException | Λάθος δεδομένα μέσα στην καταχώρηση. |

### Παραδείγματα

Εξαγωγή μιας καταχώρησης αρχείου zip με κωδικό πρόσβασης.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Δείτε επίσης

* class [SevenZipArchiveEntry](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* συνέλευση [Aspose.Zip](../../../)


