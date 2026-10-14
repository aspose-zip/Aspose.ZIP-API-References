---
title: "XarArchive.XarArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής XarArchive. Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης XarArchive."
type: docs
weight: 10
url: /el/net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(XarCompressionSettings) {#constructor}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`XarArchive`](../).

```csharp
public XarArchive(XarCompressionSettings defaultCompressionSettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| defaultCompressionSettings | XarCompressionSettings | Οι προεπιλεγμένες ρυθμίσεις συμπίεσης, εφαρμόζονται σε όλες τις καταχωρήσεις του αρχείου. |

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### Δείτε επίσης

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## XarArchive(Stream, XarLoadOptions) {#constructor_1}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`XarArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

```csharp
public XarArchive(Stream sourceStream, XarLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. Πρέπει να είναι δυνατότητα αναζήτησης. |
| loadOptions | XarLoadOptions | Οι επιλογές για τη φόρτωση του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *sourceStream* είναι null. |
| ArgumentException | *sourceStream* δεν είναι δυνατόν να γίνει αναζήτηση. |
| InvalidDataException | *sourceStream* δεν είναι έγκυρο αρχείο xar. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Open`](../../xarfileentry/open/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο.

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [XarLoadOptions](../../xarloadoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## XarArchive(string, XarLoadOptions) {#constructor_2}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`XarArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

```csharp
public XarArchive(string path, XarLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο αρχειοθήκης. |
| loadOptions | XarLoadOptions | Οι επιλογές για τη φόρτωση του αρχείου. |

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
| InvalidDataException | Το αρχείο στο *path* δεν είναι έγκυρο αρχείο xar. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Open`](../../xarfileentry/open/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο.

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [XarLoadOptions](../../xarloadoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


