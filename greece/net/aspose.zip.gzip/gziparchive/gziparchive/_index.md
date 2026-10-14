---
title: "GzipArchive.GzipArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής GzipArchive. Δημιουργεί ένα νέο αντικείμενο της κλάσης GzipArchive προετοιμασμένο για συμπίεση"
type: docs
weight: 10
url: /el/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

Δημιουργεί ένα νέο αντικείμενο της κλάσης [`GzipArchive`](../) προετοιμασμένο για συμπίεση.

```csharp
public GzipArchive()
```

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Δείτε επίσης

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_2}

Δημιουργεί ένα νέο αντικείμενο της κλάσης [`GzipArchive`](../) προετοιμασμένο για αποσυμπίεση.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| parseHeader | Boolean | Καθορίζει αν θα γίνει ανάλυση της κεφαλίδας της ροής για να εξαχθούν ιδιότητες, συμπεριλαμβανομένου του ονόματος. Έχει νόημα μόνο για ροή με δυνατότητα αναζήτησης. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *sourceStream* είναι null. |
| EndOfStreamException | *sourceStream* είναι πολύ σύντομο. |
| InvalidDataException | Το *sourceStream* έχει λανθασμένη υπογραφή. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Open`](../open/) για αποσυμπίεση.

## Παραδείγματα

Ανοίξτε ένα αρχείο από μια ροή και εξάγετέ το σε ένα `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### Δείτε επίσης

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(Stream, GzipLoadOptions) {#constructor_1}

Δημιουργεί ένα νέο αντικείμενο της κλάσης [`GzipArchive`](../) προετοιμασμένο για αποσυμπίεση.

```csharp
public GzipArchive(Stream sourceStream, GzipLoadOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| επιλογές | GzipLoadOptions | Επιλογές για τη φόρτωση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *sourceStream* είναι null. |
| EndOfStreamException | *sourceStream* είναι πολύ σύντομο. |
| InvalidDataException | Το *sourceStream* έχει λανθασμένη υπογραφή. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Open`](../open/) για αποσυμπίεση.

## Παραδείγματα

Ανοίξτε ένα αρχείο από μια ροή και εξάγετέ το σε ένα `MemoryStream`

```csharp
var ms = new MemoryStream();
GzipLoadOptions options = new GzipLoadOptions();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz"), options))
  archive.Extract(ms);
```

### Δείτε επίσης

* class [GzipLoadOptions](../../gziploadoptions/)
* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(string, GzipLoadOptions) {#constructor_3}

Δημιουργεί ένα νέο αντικείμενο της κλάσης [`GzipArchive`](../) προετοιμασμένο για αποσυμπίεση.

```csharp
public GzipArchive(string path, GzipLoadOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο αρχειοθήκης. |
| επιλογές | GzipLoadOptions | Επιλογές για τη φόρτωση του αρχείου. |

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

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Open`](../open/) για αποσυμπίεση.

## Παραδείγματα

Ανοίξτε ένα αρχείο από διαδρομή και εξάγετε το σε ένα `MemoryStream`

```csharp
var ms = new MemoryStream();
GzipLoadOptions options = new GzipLoadOptions();
using (GzipArchive archive = new GzipArchive("archive.gz", options))
  archive.Extract(ms);
```

### Δείτε επίσης

* class [GzipLoadOptions](../../gziploadoptions/)
* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_4}

Δημιουργεί ένα νέο αντικείμενο της κλάσης [`GzipArchive`](../) προετοιμασμένο για αποσυμπίεση.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο αρχειοθήκης. |
| parseHeader | Boolean | Καθορίζει αν θα γίνει ανάλυση της κεφαλίδας της ροής για να εξαχθούν ιδιότητες, συμπεριλαμβανομένου του ονόματος. Έχει νόημα μόνο για ροή με δυνατότητα αναζήτησης. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| EndOfStreamException | Το αρχείο είναι πολύ μικρό. |
| InvalidDataException | Τα δεδομένα στο αρχείο έχουν λανθασμένη υπογραφή. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [`Open`](../open/) για αποσυμπίεση.

## Παραδείγματα

Ανοίξτε ένα αρχείο από διαδρομή και εξάγετε το σε ένα `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### Δείτε επίσης

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


