---
title: "IsoArchive.IsoArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής IsoArchive. Αρχικοποιεί μια νέα παρουσία της κλάσης IsoArchive και δημιουργεί ένα κενό αρχείο ISO για την προσθήκη νέων αρχείων και φακέλων"
type: docs
weight: 10
url: /el/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`IsoArchive`](../) και δημιουργεί ένα κενό αρχείο ISO για την προσθήκη νέων αρχείων και φακέλων.

```csharp
public IsoArchive()
```

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να δημιουργήσετε ένα νέο κενό αρχείο ISO και να προσθέσετε αρχεία σε αυτό:

```csharp
// Δημιουργήστε ένα νέο κενό αρχείο ISO
using(IsoArchive isoArchive = new IsoArchive())
{
    // Προσθέστε αρχεία στο αρχείο ISO
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Αποθηκεύστε το αρχείο ISO σε ένα αρχείο
    isoArchive.Save("new_archive.iso");
}
```

### Δείτε επίσης

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`IsoArchive`](../) και συνθέτει μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. Πρέπει να είναι δυνατότητα αναζήτησης. |
| loadOptions | IsoLoadOptions | Οι επιλογές για τη φόρτωση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *sourceStream* είναι null. |
| ArgumentException | *sourceStream* δεν είναι δυνατόν να γίνει αναζήτηση. |
| InvalidDataException | *sourceStream* δεν είναι έγκυρο αρχείο ISO. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |
| EndOfStreamException | Εκτοπίζεται όταν το τέλος της ροής επιτυγχάνεται απροσδόκητα. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |
| NotSupportedException | Η ροή δεν υποστηρίζει ανάγνωση. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση.

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`IsoArchive`](../) και συνθέτει μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο αρχειοθήκης. |
| loadOptions | IsoLoadOptions | Οι επιλογές για τη φόρτωση του αρχείου. |

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
| EndOfStreamException | Το αρχείο είναι πολύ μικρό. |
| InvalidDataException | Εκτοπίζεται όταν τα δεδομένα είναι μη έγκυρα ή κατεστραμμένα. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση.

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


