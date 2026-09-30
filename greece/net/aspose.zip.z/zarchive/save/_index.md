---
title: "ZArchive.Save"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος ZArchive. Αποθηκεύει το αρχείο xz στη δοθείσα ροή."
type: docs
weight: 50
url: /el/net/aspose.zip.z/zarchive/save/
---
## Save(Stream, ZArchiveSaveOptions) {#save}

Αποθηκεύει το xz archive στη δοθείσα ροή.

```csharp
public void Save(Stream output, ZArchiveSaveOptions settings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |
| ρυθμίσεις | ZArchiveSaveOptions | Προαιρετικές ρυθμίσεις για τη σύνθεση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentException | *output* δεν υποστηρίζει αναζήτηση. |
| ArgumentNullException | *output* είναι null. |

## Παρατηρήσεις

*output* must be seekable.

## Παραδείγματα

```csharp
using (FileStream zFile = File.Open("data.bin.z", FileMode.Create))
{
    using (var archive = new ZArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(zFile);
     }
}
```

### Δείτε επίσης

* class [ZArchiveSaveOptions](../../zarchivesaveoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZArchiveSaveOptions) {#save_1}

Αποθηκεύει το Z archive στο παρεχόμενο αρχείο προορισμού.

```csharp
public void Save(string destinationFileName, ZArchiveSaveOptions settings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | +Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| ρυθμίσεις | ZArchiveSaveOptions | Προαιρετικές ρυθμίσεις για τη σύνθεση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentNullException | *destinationFileName* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Το *destinationFileName* είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *destinationFileName* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο *destinationFileName*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες στα Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *destinationFileName* περιέχει άνω-κάθετο (: ) στη μέση της συμβολοσειράς. |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά το άνοιγμα του αρχείου. |

## Παραδείγματα

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### Δείτε επίσης

* class [ZArchiveSaveOptions](../../zarchivesaveoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)


