---
title: "CabArchive.CabArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "CabArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία της κλάσης CabArchive προετοιμασμένη για συμπίεση"
type: docs
weight: 10
url: /el/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(CabEntrySettings) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`CabArchive`](../) προετοιμασμένη για συμπίεση.

```csharp
public CabArchive(CabEntrySettings settings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| settings | CabEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για τα πρόσφατα προστιθέμενα στοιχεία [`CabEntry`](../../cabentry/). Εάν δεν καθοριστούν, θα χρησιμοποιηθεί η συμπίεση MSZIP. |

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cab");
}
```

Συμπιέστε ένα αρχείο χρησιμοποιώντας συγκεκριμένες ρυθμίσεις συμπίεσης.

```csharp
using (var archive = new CabArchive())
{
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("entry.bin", "data.bin", settings);
    archive.Save("archive.cab");
}
```

### Δείτε επίσης

* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CabArchive(Stream, CabLoadOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`CabArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

```csharp
public CabArchive(Stream sourceStream, CabLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. Πρέπει να είναι δυνατότητα αναζήτησης. |
| loadOptions | CabLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *sourceStream* είναι null. |
| ArgumentException | *sourceStream* δεν είναι δυνατόν να γίνει αναζήτηση. |
| InvalidDataException | *sourceStream* δεν είναι έγκυρο αρχείο CAB. |
| EndOfStreamException | Η ροή είναι πολύ μικρή. |
| ObjectDisposedException | Εκτοξεύεται όταν η ροή έχει διαγραφεί. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |
| NotSupportedException | Η ροή δεν υποστηρίζει αναζήτηση, όπως όταν η ροή είναι κατασκευασμένη από σωλήνα ή έξοδο κονσόλας. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Open`](../../cabentry/open/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [CabLoadOptions](../../cabloadoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CabArchive(string, CabLoadOptions) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`CabArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

```csharp
public CabArchive(string path, CabLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο αρχειοθήκης. |
| loadOptions | CabLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |
| EndOfStreamException | Το αρχείο είναι πολύ μικρό. |
| InvalidDataException | Ο μαγικός αριθμός CAB είναι άκυρος ή το μέγεθος της κεφαλίδας δεν ταιριάζει. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Open`](../../cabentry/open/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο.

```csharp
using (var archive = new CabArchive("archive.cab")) hj
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [CabLoadOptions](../../cabloadoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


