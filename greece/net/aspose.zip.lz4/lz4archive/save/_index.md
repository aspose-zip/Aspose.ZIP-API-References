---
title: "Lz4Archive.Save"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Lz4Archive μέθοδος. Αποθηκεύει το αρχείο lz4 στη δοθείσα ροή"
type: docs
weight: 60
url: /el/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

Αποθηκεύει το αρχείο lz4 στη ροή που παρέχεται.

```csharp
public void Save(Stream output)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *output* είναι null. |
| ArgumentException | *output* δεν είναι εγγράψιμο. |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για εξαγωγή. - ή - Η πηγή δεν παρείχε. |
| OperationCanceledException | Στο .NET Framework 4.0 και νεότερα: Εγείρεται όταν η συμπίεση ακυρώνεται μέσω του παρεχόμενου token ακύρωσης. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παρατηρήσεις

*output* must be seekable.

## Παραδείγματα

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### Δείτε επίσης

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Αποθηκεύει το αρχείο lz4 στον προτεινόμενο αρχείο προορισμού.

```csharp
public void Save(FileInfo destination)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | FileInfo | FileInfo, το οποίο θα ανοιχτεί ως ροή προορισμού. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| SecurityException | Το πρόγραμμα που καλεί δεν έχει την απαιτούμενη άδεια για το άνοιγμα του *destination*. |
| ArgumentException | Η διαδρομή του αρχείου είναι κενή ή περιέχει μόνο κενά διαστήματα. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| UnauthorizedAccessException | Η διαδρομή προς το αρχείο είναι μόνο για ανάγνωση ή είναι κατάλογος. |
| ArgumentNullException | *destination* είναι null. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για εξαγωγή. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### Δείτε επίσης

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

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
| SecurityException | Ο καλών δεν διαθέτει τα απαιτούμενα δικαιώματα πρόσβασης. |
| ArgumentException | Το *destinationFileName* είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *destinationFileName* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο *destinationFileName*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες στα Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *destinationFileName* περιέχει άνω-κάθετο (: ) στη μέση της συμβολοσειράς. |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για εξαγωγή. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη (για παράδειγμα, βρίσκεται σε μη αντιστοιχισμένο δίσκο). |
| FileNotFoundException | Το αρχείο που καθορίστηκε στο *destinationFileName* δεν βρέθηκε. |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά το άνοιγμα του αρχείου. |

## Παραδείγματα

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Δείτε επίσης

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


