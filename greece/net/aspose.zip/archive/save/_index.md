---
title: "Archive.Save"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος Archive. Αποθηκεύει το αρχείο στη δοθείσα ροή."
type: docs
weight: 100
url: /el/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή.

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outputStream | Stream | Ροή προορισμού. |
| saveOptions | ArchiveSaveOptions | Επιλογές για την αποθήκευση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *outputStream* δεν είναι εγγράψιμο. |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί. |
| InvalidOperationException | Εκτοξεύεται όταν εφαρμόζεται κρυπτογράφηση σε ήδη κρυπτογραφημένες καταχωρήσεις. |

## Παρατηρήσεις

*outputStream* must be writable.

## Παραδείγματα

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(zipFile);
    }
}
```

### Δείτε επίσης

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

Αποθηκεύει την αρχειοθήκη στο παρεχόμενο αρχείο προορισμού

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| saveOptions | ArchiveSaveOptions | Επιλογές για την αποθήκευση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *destinationFileName* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Το *destinationFileName* είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *destinationFileName* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο *destinationFileName*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες στα Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *destinationFileName* περιέχει άνω-κάθετο (: ) στη μέση της συμβολοσειράς. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |
| ObjectDisposedException | Εκτοπίζεται εάν το αρχείο έχει διαγραφεί. |
| InvalidOperationException | Εκτοξεύεται όταν εφαρμόζεται κρυπτογράφηση σε ήδη κρυπτογραφημένες καταχωρήσεις. |

## Παρατηρήσεις

Είναι δυνατόν να αποθηκεύσετε ένα αρχείο στην ίδια διαδρομή από την οποία φορτώθηκε. Ωστόσο, αυτό δεν συνιστάται επειδή αυτή η προσέγγιση χρησιμοποιεί αντιγραφή σε προσωρινό αρχείο.

## Παραδείγματα

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Δείτε επίσης

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


