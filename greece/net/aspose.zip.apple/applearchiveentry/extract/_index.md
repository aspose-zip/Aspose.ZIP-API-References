---
title: "AppleArchiveEntry.Extract"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "AppleArchiveEntry μέθοδος. Εξάγει την καταχώρηση στο σύστημα αρχείων με τη δοθείσα διαδρομή"
type: docs
weight: 50
url: /el/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

Εξάγει την καταχώρηση στο σύστημα αρχείων με τη δοθείσα διαδρομή.

```csharp
public FileInfo Extract(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidDataException | Το άθροισμα ελέγχου ή η σύνοψη που αποθηκεύτηκε για την καταχώρηση δεν ταιριάζει με τα εξαγμένα δεδομένα. |
| InvalidOperationException | Η καταχώρηση ανήκει σε ένα αρχείο που έχει προετοιμαστεί για σύνθεση, ή τα δεδομένα της καταχώρησης δεν μπορούν να ανοιχτούν από ένα μη αναζητήσιμο ρεύμα αρχείου. |
| NotSupportedException | Η καταχώρηση ανήκει σε ένα συμπαγές Apple Archive ή χρησιμοποιεί μια μη υποστηριζόμενη μέθοδο συμπίεσης. |
| ObjectDisposedException | Το πηγαίο ρεύμα έχει διαγραφεί. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |

### Δείτε επίσης

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
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
| ArgumentNullException | *destination* είναι `null`. |
| ArgumentException | *destination* δεν υποστηρίζει εγγραφή. |
| InvalidDataException | Το άθροισμα ελέγχου ή η σύνοψη που αποθηκεύτηκε για την καταχώρηση δεν ταιριάζει με τα εξαγμένα δεδομένα. |
| InvalidOperationException | Η καταχώρηση ανήκει σε ένα αρχείο που έχει προετοιμαστεί για σύνθεση, ή τα δεδομένα της καταχώρησης δεν μπορούν να ανοιχτούν από ένα μη αναζητήσιμο ρεύμα αρχείου. |
| NotSupportedException | Η καταχώρηση ανήκει σε ένα συμπαγές Apple Archive ή χρησιμοποιεί μια μη υποστηριζόμενη μέθοδο συμπίεσης. |
| ObjectDisposedException | Το πηγαίο ρεύμα έχει διαγραφεί. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |

### Δείτε επίσης

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


