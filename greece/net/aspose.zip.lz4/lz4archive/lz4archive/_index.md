---
title: "Lz4Archive.Lz4Archive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής Lz4Archive. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης Lz4Archive προετοιμασμένο για αποσυμπίεση"
type: docs
weight: 10
url: /el/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Lz4Archive`](../) προετοιμασμένο για αποσυμπίεση.

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| loadOptions | Lz4LoadOptions | Οι επιλογές για τη φόρτωση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | Αδυναμία ανάγνωσης από *sourceStream* |
| ArgumentNullException | *sourceStream* είναι null. |
| EndOfStreamException | *sourceStream* είναι πολύ σύντομο. |
| InvalidDataException | Το *sourceStream* έχει λανθασμένη υπογραφή. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Open`](../open/) για αποσυμπίεση.

## Παραδείγματα

Ανοίξτε ένα αρχείο από μια ροή και εξάγετέ το σε ένα `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### Δείτε επίσης

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Lz4Archive`](../).

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο αρχειοθήκης. |
| loadOptions | Lz4LoadOptions | Οι επιλογές για τη φόρτωση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Ο καλών δεν διαθέτει τα απαιτούμενα δικαιώματα πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| EndOfStreamException | Το αρχείο είναι πολύ μικρό. |
| InvalidDataException | Τα δεδομένα στο αρχείο έχουν λανθασμένη υπογραφή. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Open`](../open/) για αποσυμπίεση.

## Παραδείγματα

Ανοίξτε ένα αρχείο από διαδρομή και εξάγετε το σε ένα `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### Δείτε επίσης

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Lz4Archive`](../) προετοιμασμένο για συμπίεση.

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ρυθμίσεις | Lz4ArchiveSetting | Η ρύθμιση του σύνθετου αρχείου. |

### Δείτε επίσης

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


