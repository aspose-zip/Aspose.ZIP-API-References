---
title: "XarArchive.Save"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος XarArchive. Αποθηκεύει το αρχείο στο αρχείο προορισμού που παρέχεται."
type: docs
weight: 80
url: /el/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

Αποθηκεύει την αρχειοθήκη στο παρεχόμενο αρχείο προορισμού

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| saveOptions | XarSaveOptions | Επιλογές για την αποθήκευση του αρχείου xar. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *destinationFileName* είναι null. |
| InvalidOperationException | Αδύνατη η τροποποίηση του αρχείου xar. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά το άνοιγμα του αρχείου. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. |
| UnauthorizedAccessException | *destinationFileName* καθόρισε ένα αρχείο που είναι μόνο για ανάγνωση. -ή- *destinationFileName* καθόρισε έναν φάκελο. -ή- Ο καλών δεν διαθέτει την απαιτούμενη άδεια. |

### Δείτε επίσης

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |
| saveOptions | XarSaveOptions | Επιλογές για την αποθήκευση του αρχείου xar. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *output* είναι null. |
| ArgumentException | *output* δεν είναι εγγράψιμο/αναγνώσιμο ή δεν υποστηρίζει αναζήτηση. |
| InvalidOperationException | Αδύνατη η τροποποίηση του αρχείου xar. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

### Δείτε επίσης

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


