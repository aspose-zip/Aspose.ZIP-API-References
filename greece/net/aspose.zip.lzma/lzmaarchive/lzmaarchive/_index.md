---
title: "LzmaArchive.LzmaArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "LzmaArchive κατασκευαστής. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης LzmaArchive και δημιουργεί το αρχείο σε μορφή lzma"
type: docs
weight: 10
url: /el/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`LzmaArchive`](../) και δημιουργεί το αρχείο σε μορφή lzma.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ρυθμίσεις | LzmaArchiveSettings | Σύνολο ρυθμίσεων για συγκεκριμένο αρχείο lzma. |

### Δείτε επίσης

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`LzmaArchive`](../) προετοιμασμένο για αποσυμπίεση.

```csharp
public LzmaArchive(Stream source)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | Stream | Η πηγή του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *source* είναι null. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Extract`](../extract/) για αποσυμπίεση.

### Δείτε επίσης

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`LzmaArchive`](../) προετοιμασμένο για αποσυμπίεση.

```csharp
public LzmaArchive(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Διαδρομή προς την πηγή του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Extract`](../extract/) για αποσυμπίεση.

## Παραδείγματα

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
}
```

### Δείτε επίσης

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)


