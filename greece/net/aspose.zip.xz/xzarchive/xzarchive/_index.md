---
title: "XzArchive.XzArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής XzArchive. Αρχικοποιεί μια νέα παρουσία της κλάσης XzArchive και δημιουργεί το αρχείο σε μορφή xz"
type: docs
weight: 10
url: /el/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`XzArchive`](../) και δημιουργεί το αρχείο σε μορφή xz.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ρυθμίσεις | XzArchiveSettings | Σύνολο ρυθμίσεων συγκεκριμένου αρχείου xz: μέγεθος λεξικού, μέγεθος μπλοκ, τύπος ελέγχου. |

### Δείτε επίσης

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## XzArchive(Stream, XzLoadOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`XzArchive`](../) προετοιμασμένη για αποσυμπίεση.

```csharp
public XzArchive(Stream source, XzLoadOptions options = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | Stream | Η πηγή του αρχείου. |
| επιλογές | XzLoadOptions | Επιλογές για τη φόρτωση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *source* δεν είναι δυνατόν να γίνει αναζήτηση. |
| ArgumentNullException | *source* είναι null. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |
| InvalidDataException | Τα δεδομένα είναι άκυρα ή κατεστραμμένα. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Extract`](../extract/) για αποσυμπίεση.

### Δείτε επίσης

* class [XzLoadOptions](../../../aspose.zip.xz.settings/xzloadoptions/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## XzArchive(string, XzLoadOptions) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`XzArchive`](../) προετοιμασμένη για αποσυμπίεση.

```csharp
public XzArchive(string path, XzLoadOptions options = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Διαδρομή προς την πηγή του αρχείου. |
| επιλογές | XzLoadOptions | Επιλογές για τη φόρτωση του αρχείου. |

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
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| InvalidDataException | Εκτοπίζεται όταν τα δεδομένα είναι μη έγκυρα ή κατεστραμμένα. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Extract`](../extract/) για αποσυμπίεση.

### Δείτε επίσης

* class [XzLoadOptions](../../../aspose.zip.xz.settings/xzloadoptions/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)


