---
title: "GzipArchive.Save"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "GzipArchive μέθοδος. Αποθηκεύει το αρχείο στη δοθείσα ροή"
type: docs
weight: 80
url: /el/net/aspose.zip.gzip/gziparchive/save/
---
## Save(Stream) {#save}

Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή.

```csharp
public void Save(Stream outputStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outputStream | Stream | Ροή προορισμού. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *outputStream* δεν είναι εγγράψιμο. |
| InvalidOperationException | Δεν έχει παρασχεθεί η πηγή. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παρατηρήσεις

*outputStream* must be writable.

## Παραδείγματα

Γράφει τα συμπιεσμένα δεδομένα στη ροή απόκρισης http.

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Δείτε επίσης

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Αποθηκεύει την αρχειοθήκη στο παρεχόμενο αρχείο προορισμού

```csharp
public void Save(string destinationFileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *destinationFileName* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Το *destinationFileName* είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *destinationFileName* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο *destinationFileName*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες στα Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *destinationFileName* περιέχει άνω-κάθετο (: ) στη μέση της συμβολοσειράς. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Δείτε επίσης

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


