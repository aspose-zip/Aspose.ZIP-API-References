---
title: TarEntry.Extract
second_title: Aspose.ZIP για Αναφορά API .NET
description: TarEntry μέθοδος. Εξάγει την καταχώρηση στο σύστημα αρχείων από τη διαδρομή που παρέχεται.
type: docs
weight: 40
url: /el/net/aspose.zip.tar/tarentry/extract/
---
## Extract(string) {#extract}

Εξάγει την καταχώρηση στο σύστημα αρχείων από τη διαδρομή που παρέχεται.

```csharp
public FileSystemInfo Extract(string path)
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
using (var archive = new TarArchive("archive.tar"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Δείτε επίσης

* class [TarEntry](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tarentry/)
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

Εξαγωγή μιας καταχώρησης αρχείου πίσσας.

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Δείτε επίσης

* class [TarEntry](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tarentry/)
* συνέλευση [Aspose.Zip](../../../)


