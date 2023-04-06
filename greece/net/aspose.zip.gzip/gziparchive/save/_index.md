---
title: GzipArchive.Save
second_title: Aspose.ZIP για Αναφορά API .NET
description: GzipArchive μέθοδος. Αποθηκεύει το αρχείο στη ροή που παρέχεται.
type: docs
weight: 60
url: /el/net/aspose.zip.gzip/gziparchive/save/
---
## Save(Stream) {#save}

Αποθηκεύει το αρχείο στη ροή που παρέχεται.

```csharp
public void Save(Stream outputStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outputStream | Stream | Ροή προορισμού. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *outputStream* δεν είναι εγγράψιμο. |
| InvalidOperationException | Η πηγή δεν έχει παρασχεθεί. |

### Παρατηρήσεις

*outputStream*πρέπει να είναι εγγράψιμο.

### Παραδείγματα

Εγγράφει συμπιεσμένα δεδομένα στη ροή απόκρισης http.

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Δείτε επίσης

* class [GzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Gzip](../../gziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Αποθηκεύει το αρχείο στο παρεχόμενο αρχείο προορισμού.

```csharp
public void Save(string destinationFileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου παραπέμπει σε ένα υπάρχον αρχείο, θα αντικατασταθεί. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *destinationFileName* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*destinationFileName* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*destinationFileName* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*destinationFileName*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*destinationFileName* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |

### Παραδείγματα

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Δείτε επίσης

* class [GzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Gzip](../../gziparchive/)
* συνέλευση [Aspose.Zip](../../../)


