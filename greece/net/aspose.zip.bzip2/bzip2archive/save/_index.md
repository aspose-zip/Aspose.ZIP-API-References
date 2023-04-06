---
title: Bzip2Archive.Save
second_title: Aspose.ZIP για Αναφορά API .NET
description: Bzip2Archive μέθοδος. Αποθηκεύει το αρχείο στη ροή που παρέχεται.
type: docs
weight: 50
url: /el/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

Αποθηκεύει το αρχείο στη ροή που παρέχεται.

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outputStream | Stream | Ροή προορισμού. |
| saveOptions | Bzip2SaveOptions | Επιλογές για την αποθήκευση ενός αρχείου bzip2. Εάν δεν καθορίζεται, θα χρησιμοποιηθεί μέγεθος μπλοκ 900 Kb. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| InvalidOperationException | Η πηγή των δεδομένων που πρόκειται να αρχειοθετηθούν δεν έχει παρασχεθεί. |
| ArgumentException | *outputStream* δεν είναι εγγράψιμο. |
| UnauthorizedAccessException | Η πηγή αρχείου είναι μόνο για ανάγνωση ή είναι κατάλογος. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή προέλευσης αρχείου δεν είναι έγκυρη, όπως είναι σε μη αντιστοιχισμένη μονάδα δίσκου. |
| IOException | Η πηγή αρχείου είναι ήδη ανοιχτή. |

### Παρατηρήσεις

*outputStream*πρέπει να είναι εγγράψιμο.

### Παραδείγματα

Εγγράφει συμπιεσμένα δεδομένα στη ροή απόκρισης http.

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
* χώρος ονομάτων [Aspose.Zip.Bzip2](../../bzip2archive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

Αποθηκεύει το αρχείο στο παρεχόμενο αρχείο προορισμού.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου παραπέμπει σε ένα υπάρχον αρχείο, θα αντικατασταθεί. |
| saveOptions | Bzip2SaveOptions | Επιλογές για την αποθήκευση ενός αρχείου bzip2. Εάν δεν καθορίζεται, θα χρησιμοποιηθεί μέγεθος μπλοκ 900 Kb. |

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

Γράφει συμπιεσμένα δεδομένα στο αρχείο.

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
* χώρος ονομάτων [Aspose.Zip.Bzip2](../../bzip2archive/)
* συνέλευση [Aspose.Zip](../../../)


