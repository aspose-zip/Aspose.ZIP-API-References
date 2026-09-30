---
title: "LzipArchive.LzipArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "LzipArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία του LzipArchive"
type: docs
weight: 10
url: /el/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

Αρχικοποιεί μια νέα παρουσία του [`LzipArchive`](../).

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ρυθμίσεις | LzipArchiveSettings | Ρύθμιση συγκεκριμένου lzip αρχείου με ορισμό του μεγέθους λεξικού. |

### Δείτε επίσης

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## LzipArchive(Stream, LzipLoadOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LzipArchive`](../) προετοιμασμένη για αποσυμπίεση.

```csharp
public LzipArchive(Stream sourceStream, LzipLoadOptions options = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| επιλογές | LzipLoadOptions | Επιλογές για τη φόρτωση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *sourceStream* δεν είναι δυνατόν να γίνει αναζήτηση. |
| ArgumentNullException | *sourceStream* είναι null. |
| InvalidDataException | Οι κεφαλίδες δεν ταιριάζουν με τον τύπο lzip του αρχείου. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Extract`](../extract/) για αποσυμπίεση.

### Δείτε επίσης

* class [LzipLoadOptions](../../lziploadoptions/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## LzipArchive(string, LzipLoadOptions) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LzipArchive`](../) προετοιμασμένη για αποσυμπίεση.

```csharp
public LzipArchive(string path, LzipLoadOptions options = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Διαδρομή προς την πηγή του αρχείου. |
| επιλογές | LzipLoadOptions | Επιλογές για τη φόρτωση του αρχείου. |

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
| InvalidDataException | Οι κεφαλίδες δεν ταιριάζουν με τον τύπο lzip του αρχείου. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Extract`](../extract/) για αποσυμπίεση.

## Παραδείγματα

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### Δείτε επίσης

* class [LzipLoadOptions](../../lziploadoptions/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)


