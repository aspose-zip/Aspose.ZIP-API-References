---
title: CabEntry.Extract
second_title: Aspose.ZIP για Αναφορά API .NET
description: CabEntry μέθοδος. Εξάγει την καταχώρηση στο σύστημα αρχείων από τη διαδρομή που παρέχεται.
type: docs
weight: 30
url: /el/net/aspose.zip.cab/cabentry/extract/
---
## Extract(string) {#extract}

Εξάγει την καταχώρηση στο σύστημα αρχείων από τη διαδρομή που παρέχεται.

```csharp
public FileInfo Extract(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί. |

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
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Δείτε επίσης

* class [CabEntry](../)
* χώρος ονομάτων [Aspose.Zip.Cab](../../cabentry/)
* συνέλευση [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Εξάγει την καταχώρηση στη ροή που παρέχεται.

```csharp
public void Extract(Stream destination)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destination | Stream | Ροή προορισμού. Πρέπει να είναι εγγράψιμο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *destination* δεν υποστηρίζει τη γραφή. |

### Παραδείγματα

Εξαγάγετε μια καταχώρηση του αρχείου ταξί.

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Δείτε επίσης

* class [CabEntry](../)
* χώρος ονομάτων [Aspose.Zip.Cab](../../cabentry/)
* συνέλευση [Aspose.Zip](../../../)


