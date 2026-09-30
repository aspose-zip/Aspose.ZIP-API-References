---
title: "IsoArchive.Save"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος IsoArchive. Αποθηκεύει την εικόνα ISO στην καθορισμένη διαδρομή"
type: docs
weight: 70
url: /el/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

Αποθηκεύει την εικόνα ISO στην καθορισμένη διαδρομή.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή όπου θα αποθηκευτεί η εικόνα ISO. |
| saveOptions | IsoSaveOptions | Επιλογές για την αποθήκευση του αρχείου ISO. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εκτοπίζεται όταν το αρχείο δεν βρίσκεται σε λειτουργία επεξεργασίας. |
| ArgumentNullException | Εκτοπίζεται όταν η *path* είναι null. |
| DirectoryNotFoundException | Εκτοπίζεται όταν η καθορισμένη διαδρομή είναι άκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Εκτοπίζεται όταν το αρχείο είναι ήδη ανοιχτό. |
| UnauthorizedAccessException | Εκτοπίζεται όταν η πρόσβαση στη *διαδρομή* του αρχείου απορρίπτεται. |
| PathTooLongException | Εκτοπίζεται όταν η καθορισμένη *διαδρομή* υπερβαίνει το μέγιστο μήκος που ορίζεται από το σύστημα. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να αποθηκεύσετε ένα αρχείο ISO σε ένα αρχείο:

```csharp
// Δημιουργήστε ένα νέο κενό αρχείο ISO
using(IsoArchive isoArchive = new IsoArchive())
{
    // Προσθέστε αρχεία στο αρχείο ISO
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Αποθηκεύστε το αρχείο ISO σε ένα αρχείο
    isoArchive.Save("new_archive.iso");
}
```

### Δείτε επίσης

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

Αποθηκεύει την εικόνα ISO στην καθορισμένη ροή.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή όπου θα αποθηκευτεί η εικόνα ISO. |
| saveOptions | IsoSaveOptions | Επιλογές για την αποθήκευση του αρχείου ISO. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εκτοπίζεται όταν το αρχείο δεν βρίσκεται σε λειτουργία επεξεργασίας. |
| ArgumentNullException | Εκτοπίζεται όταν η *ροή* είναι null. |
| ArgumentException | Εκτοπίζεται όταν η *ροή* δεν είναι εγγράψιμη. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να αποθηκεύσετε ένα αρχείο ISO σε ροή μνήμης:

```csharp

 // Δημιουργήστε ένα νέο κενό αρχείο ISO
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // Προσθέστε αρχεία στο αρχείο ISO
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // Αποθηκεύστε το αρχείο ISO σε ροή μνήμης
     isoArchive.Save(memoryStream);
 }
```

### Δείτε επίσης

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


