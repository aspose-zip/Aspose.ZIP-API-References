---
title: "RarArchive.RarArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής RarArchive. Αρχικοποιεί μια νέα παρουσία της κλάσης RarArchive και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο"
type: docs
weight: 10
url: /el/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`RarArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η πλήρης ή σχετική διαδρομή προς το αρχείο του αρχείου. |
| loadOptions | RarArchiveLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

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
| InvalidDataException | Εκτοπίζεται όταν τα δεδομένα είναι μη έγκυρα ή κατεστραμμένα. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Open`](../../rararchiveentry/open/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα εξάγει ένα αρχείο, στη συνέχεια αποσυμπιέζει την πρώτη καταχώρηση σε ένα `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Δείτε επίσης

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* namespace [Aspose.Zip.Rar](../../rararchive/)
* assembly [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`RarArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| loadOptions | RarArchiveLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *sourceStream* δεν είναι δυνατόν να γίνει αναζήτηση. |
| InvalidDataException | Λάθος υπογραφή για το αρχείο. - ή - Το αρχείο δεν είναι αρχείο RAR. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`Open`](../../rararchiveentry/open/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα αποκρυπτογραφεί και αποσυμπιέζει την πρώτη καταχώρηση σε ένα `MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Δείτε επίσης

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* namespace [Aspose.Zip.Rar](../../rararchive/)
* assembly [Aspose.Zip](../../../)


