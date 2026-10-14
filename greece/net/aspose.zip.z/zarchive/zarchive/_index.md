---
title: "ZArchive.ZArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής ZArchive. Αρχικοποιεί μια νέα παρουσία της κλάσης ZArchive προετοιμασμένη για συμπίεση"
type: docs
weight: 10
url: /el/net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`ZArchive`](../) προετοιμασμένη για συμπίεση.

```csharp
public ZArchive()
```

### Δείτε επίσης

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZArchive(Stream, ZArchiveLoadOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`ZArchive`](../) προετοιμασμένη για αποσυμπίεση.

```csharp
public ZArchive(Stream source, ZArchiveLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | Stream | Η πηγή του αρχείου. |
| loadOptions | ZArchiveLoadOptions | Οι επιλογές για τη φόρτωση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *source* δεν είναι δυνατόν να γίνει αναζήτηση. |
| ArgumentNullException | *source* είναι null. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Extract`](../extract/) για αποσυμπίεση.

### Δείτε επίσης

* class [ZArchiveLoadOptions](../../zarchiveloadoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZArchive(string, ZArchiveLoadOptions) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`ZArchive`](../) προετοιμασμένη για αποσυμπίεση.

```csharp
public ZArchive(string path, ZArchiveLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Διαδρομή προς την πηγή του αρχείου. |
| loadOptions | ZArchiveLoadOptions | Οι επιλογές για τη φόρτωση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Extract`](../extract/) για αποσυμπίεση.

### Δείτε επίσης

* class [ZArchiveLoadOptions](../../zarchiveloadoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)


