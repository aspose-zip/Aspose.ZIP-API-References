---
title: "TarArchive.TarArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής TarArchive. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης TarArchive"
type: docs
weight: 10
url: /el/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`TarArchive`](../).

```csharp
public TarArchive()
```

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### Δείτε επίσης

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## TarArchive(Stream, TarLoadOptions) {#constructor_1}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`TarArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

```csharp
public TarArchive(Stream sourceStream, TarLoadOptions loadOptions = null)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| sourceStream | Η πηγή του αρχείου. Πρέπει να είναι δυνατότητα αναζήτησης. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *sourceStream* δεν είναι δυνατόν να γίνει αναζήτηση. |
| ArgumentNullException | *sourceStream* είναι null. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Open`](../../tarentry/open/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [TarLoadOptions](../../tarloadoptions/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## TarArchive(string, TarLoadOptions) {#constructor_2}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`TarArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

```csharp
public TarArchive(string path, TarLoadOptions loadOptions = null)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| διαδρομή | Η διαδρομή προς το αρχείο αρχειοθήκης. |

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

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Open`](../../tarentry/open/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο.

```csharp
using (var archive = new TarArchive("archive.tar", new TarLoadOptions() { CancellationToken = cancellationToken }))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [TarLoadOptions](../../tarloadoptions/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


