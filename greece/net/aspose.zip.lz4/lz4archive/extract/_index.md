---
title: "Lz4Archive.Extract"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος Lz4Archive. Εξάγει το αρχείο στη διαδρομή που δίνεται."
type: docs
weight: 30
url: /el/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

Εξάγει το αρχείο στο αρχείο με βάση τη διαδρομή.

```csharp
public FileInfo Extract(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί. |

### Τιμή Επιστροφής

Πληροφορίες ενός εξαγόμενου αρχείου.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| EndOfStreamException | Η πηγή ροής είναι πολύ μικρή. |
| InvalidDataException | Βρέθηκαν εσφαλμένα byte κατά την αποκωδικοποίηση. |
| NotSupportedException | Αυτή η έκδοση LZ4 δεν υποστηρίζεται. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για σύνθεση. |

### Δείτε επίσης

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Εξάγει το αρχείο στο παρεχόμενο ρεύμα.

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
| EndOfStreamException | Η πηγή ροής είναι πολύ μικρή. |
| InvalidDataException | Βρέθηκαν εσφαλμένα byte κατά την αποκωδικοποίηση. |
| NotSupportedException | Αυτή η έκδοση LZ4 δεν υποστηρίζεται. |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για σύνθεση. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### Δείτε επίσης

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


