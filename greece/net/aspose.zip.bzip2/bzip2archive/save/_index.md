---
title: "Bzip2Archive.Save"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Bzip2Archive method. Αποθηκεύει το αρχείο στην παρεχόμενη ροή."
type: docs
weight: 60
url: /el/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή.

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outputStream | Stream | Ροή προορισμού. |
| saveOptions | Bzip2SaveOptions | Επιλογές για την αποθήκευση ενός αρχείου bzip2. Εάν δεν καθοριστεί, θα χρησιμοποιηθεί μέγεθος μπλοκ 900 Kb. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Η πηγή των δεδομένων που θα αρχειοθετηθούν δεν έχει παρασχεθεί. |
| ArgumentException | *outputStream* δεν είναι εγγράψιμο. |
| UnauthorizedAccessException | Η πηγή του αρχείου είναι μόνο για ανάγνωση ή είναι κατάλογος. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή πηγής αρχείου είναι άκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Η πηγή του αρχείου είναι ήδη ανοιχτή. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παρατηρήσεις

*outputStream* must be writable.

## Παραδείγματα

Γράψτε τα συμπιεσμένα δεδομένα στο ρεύμα απόκρισης http.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Δείτε επίσης

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

Αποθηκεύει το αρχείο σε προορισμένο αρχείο που παρέχεται.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| saveOptions | Bzip2SaveOptions | Επιλογές για την αποθήκευση ενός αρχείου bzip2. Εάν δεν καθοριστεί, θα χρησιμοποιηθεί μέγεθος μπλοκ 900 Kb. |

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
| InvalidOperationException | Η πηγή των δεδομένων που θα αρχειοθετηθούν δεν έχει παρασχεθεί. |

## Παραδείγματα

Γράφει τα συμπιεσμένα δεδομένα σε αρχείο.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### Δείτε επίσης

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


