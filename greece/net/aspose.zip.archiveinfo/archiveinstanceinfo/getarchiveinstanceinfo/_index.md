---
title: "ArchiveInstanceInfo.GetArchiveInstanceInfo"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος ArchiveInstanceInfo. Επιστρέφει πληροφορίες στιγμιότυπου αρχείου"
type: docs
weight: 10
url: /el/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

Λαμβάνει πληροφορίες στιγμιότυπου του αρχείου.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Το όνομα αρχείου του αρχείου αρχειοθέτησης. |

### Τιμή Επιστροφής

Πληροφορίες σχετικά με το στιγμιότυπο του αρχείου ή null εάν δεν εντοπίστηκε μορφή

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *fileName* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Το *fileName* είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *fileName* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο *fileName* υπερβαίνει το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *fileName* περιέχει άνω-κάτω τελεία (:) στη μέση της συμβολοσειράς. |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά το άνοιγμα του αρχείου. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη (για παράδειγμα, βρίσκεται σε μη αντιστοιχισμένο δίσκο). |
| FileNotFoundException | Το καθορισμένο αρχείο δεν βρέθηκε. |

### Δείτε επίσης

* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

Λαμβάνει πληροφορίες στιγμιότυπου του αρχείου.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή του αρχείου αρχειοθήκης. |

### Τιμή Επιστροφής

Πληροφορίες σχετικά με το στιγμιότυπο του αρχείου ή null εάν δεν εντοπίστηκε μορφή

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *stream* είναι null. |
| ArgumentException | *stream* δεν είναι δυνατόν να γίνει αναζήτηση. |

### Δείτε επίσης

* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)


