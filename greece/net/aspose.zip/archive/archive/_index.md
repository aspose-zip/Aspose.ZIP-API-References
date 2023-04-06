---
title: Archive.Archive
second_title: Aspose.ZIP για Αναφορά API .NET
description: Archive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουArchive τάξη με προαιρετικές ρυθμίσεις για τις καταχωρήσεις της.
type: docs
weight: 10
url: /el/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`Archive`](../) τάξη με προαιρετικές ρυθμίσεις για τις καταχωρήσεις της.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για τις νέες προσθήκες[`ArchiveEntry`](../../archiveentry/) αντικείμενα. Εάν δεν καθορίζεται, θα χρησιμοποιηθεί η πιο κοινή συμπίεση Deflate χωρίς κρυπτογράφηση. |

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να συμπιέσετε ένα μεμονωμένο αρχείο με προεπιλεγμένες ρυθμίσεις.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Δείτε επίσης

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`Archive`](../) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| loadOptions | ArchiveLoadOptions | Επιλογές για τη φόρτωση του υπάρχοντος αρχείου. |
| newEntrySettings | ArchiveEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για τις νέες προσθήκες[`ArchiveEntry`](../../archiveentry/) αντικείμενα. Εάν δεν καθορίζεται, θα χρησιμοποιηθεί η πιο κοινή συμπίεση Deflate χωρίς κρυπτογράφηση. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *sourceStream* δεν είναι αναζητήσιμο. |
| InvalidDataException | Η κεφαλίδα κρυπτογράφησης για το AES έρχεται σε αντίθεση με τη μέθοδο συμπίεσης WinZip. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Βλέπω[`Open`](../../archiveentry/open/) μέθοδος αποσυμπίεσης.

### Παραδείγματα

Το ακόλουθο παράδειγμα εξάγει ένα κρυπτογραφημένο αρχείο και, στη συνέχεια, αποσυμπιέζει την πρώτη καταχώρηση στο a`MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`Archive`](../) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η πλήρως πιστοποιημένη ή η σχετική διαδρομή προς το αρχείο αρχειοθέτησης. |
| loadOptions | ArchiveLoadOptions | Επιλογές για τη φόρτωση του υπάρχοντος αρχείου. |
| newEntrySettings | ArchiveEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για τις νέες προσθήκες[`ArchiveEntry`](../../archiveentry/) αντικείμενα. Εάν δεν καθορίζεται, θα χρησιμοποιηθεί η πιο κοινή συμπίεση Deflate χωρίς κρυπτογράφηση. |

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

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Βλέπω[`Open`](../../archiveentry/open/) μέθοδος αποσυμπίεσης.

### Παραδείγματα

Το ακόλουθο παράδειγμα εξάγει ένα κρυπτογραφημένο αρχείο και, στη συνέχεια, αποσυμπιέζει την πρώτη καταχώρηση στο a`MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)


