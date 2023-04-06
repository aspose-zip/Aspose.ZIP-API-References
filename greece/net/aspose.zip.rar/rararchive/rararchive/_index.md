---
title: RarArchive.RarArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: RarArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουRarArchive Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.
type: docs
weight: 10
url: /el/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`RarArchive`](../) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η πλήρως πιστοποιημένη ή η σχετική διαδρομή προς το αρχείο αρχειοθέτησης. |
| loadOptions | RarArchiveLoadOptions | Επιλογές για τη φόρτωση του υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *path* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*path* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*path* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*path*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*path* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Βλέπω[`Open`](../../rararchiveentry/open/) μέθοδος αποσυμπίεσης.

### Παραδείγματα

Το ακόλουθο παράδειγμα εξάγει ένα αρχείο και, στη συνέχεια, αποσυμπιέζει την πρώτη καταχώρηση στο a`MemoryStream`.

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
* χώρος ονομάτων [Aspose.Zip.Rar](../../rararchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`RarArchive`](../) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| loadOptions | RarArchiveLoadOptions | Επιλογές για τη φόρτωση του υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *sourceStream* δεν είναι αναζητήσιμο. |
| InvalidDataException | Λάθος υπογραφή για αρχείο. - ή - Το αρχείο δεν είναι αρχείο RAR. |
| InvalidOperationException |  |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Βλέπω[`Open`](../../rararchiveentry/open/) μέθοδος αποσυμπίεσης.

### Παραδείγματα

Το ακόλουθο παράδειγμα αποκρυπτογραφεί και αποσυμπιέζει την πρώτη καταχώρηση στο a`MemoryStream`.

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
* χώρος ονομάτων [Aspose.Zip.Rar](../../rararchive/)
* συνέλευση [Aspose.Zip](../../../)


