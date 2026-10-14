---
title: "Archive.Archive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής Archive. Δημιουργεί ένα νέο στιγμιότυπο της κλάσης Archive με προαιρετικές ρυθμίσεις για τις καταχωρίσεις της"
type: docs
weight: 10
url: /el/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Δημιουργεί ένα νέο στιγμιότυπο της κλάσης [`Archive`](../) με προαιρετικές ρυθμίσεις για τις καταχωρίσεις της.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για τα πρόσφατα προστιθέμενα στοιχεία [`ArchiveEntry`](../../archiveentry/). Εάν δεν καθοριστούν, θα χρησιμοποιηθεί η πιο κοινή συμπίεση Deflate χωρίς κρυπτογράφηση. |

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα μόνο αρχείο με τις προεπιλεγμένες ρυθμίσεις.

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
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Δημιουργεί ένα νέο στιγμιότυπο της κλάσης [`Archive`](../) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| loadOptions | ArchiveLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |
| newEntrySettings | ArchiveEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για τα πρόσφατα προστιθέμενα στοιχεία [`ArchiveEntry`](../../archiveentry/). Εάν δεν καθοριστούν, θα χρησιμοποιηθεί η πιο κοινή συμπίεση Deflate χωρίς κρυπτογράφηση. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *sourceStream* δεν είναι δυνατόν να γίνει αναζήτηση, όταν φορτώνεται χωρίς να έχει οριστεί το [`ForwardOnly`](../../archiveloadoptions/forwardonly/). |
| InvalidDataException | Η κεφαλίδα κρυπτογράφησης για AES αντιτίθεται στη μέθοδο συμπίεσης WinZip. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| NotSupportedException | Εκτοπίζεται όταν το αρχείο φορτώνεται από ροή μόνο για ανάγνωση σε λειτουργία αξιολόγησης. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώριση. Δείτε τη μέθοδο [`Open`](../../archiveentry/open/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα εξάγει ένα κρυπτογραφημένο αρχείο, στη συνέχεια αποσυμπιέζει την πρώτη καταχώριση σε ένα `MemoryStream`.

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
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Δημιουργεί ένα νέο στιγμιότυπο της κλάσης [`Archive`](../) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η πλήρης ή σχετική διαδρομή προς το αρχείο του αρχείου. |
| loadOptions | ArchiveLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |
| newEntrySettings | ArchiveEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για τα πρόσφατα προστιθέμενα στοιχεία [`ArchiveEntry`](../../archiveentry/). Εάν δεν καθοριστούν, θα χρησιμοποιηθεί η πιο κοινή συμπίεση Deflate χωρίς κρυπτογράφηση. |

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
| InvalidDataException | Το αρχείο είναι κατεστραμμένο. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώριση. Δείτε τη μέθοδο [`Open`](../../archiveentry/open/) για αποσυμπίεση.

## Παραδείγματα

Το παρακάτω παράδειγμα εξάγει ένα κρυπτογραφημένο αρχείο, στη συνέχεια αποσυμπιέζει την πρώτη καταχώριση σε ένα `MemoryStream`.

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
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Archive(string, string[], ArchiveLoadOptions) {#constructor_3}

Δημιουργεί ένα νέο στιγμιότυπο της κλάσης [`Archive`](../) από αρχείο ZIP πολλαπλών τόμων και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο.

```csharp
public Archive(string mainSegment, string[] segmentsInOrder, ArchiveLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| mainSegment | String | Διαδρομή προς το τελευταίο τμήμα του αρχείου πολλαπλών τόμων με τον κεντρικό κατάλογο. |
| segmentsInOrder | String[] | Διαδρομές προς κάθε τμήμα εκτός του τελευταίου του αρχείο zip πολλαπλών τόμων, τηρώντας τη σειρά. |
| loadOptions | ArchiveLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| EndOfStreamException | Δεν είναι δυνατή η φόρτωση των κεφαλίδων ZIP επειδή τα παρεχόμενα αρχεία είναι κατεστραμμένα. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη (για παράδειγμα, βρίσκεται σε μη αντιστοιχισμένο δίσκο). |
| FileNotFoundException | Το αρχείο που καθορίστηκε στη διαδρομή δεν βρέθηκε. |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά το άνοιγμα του αρχείου. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. |
| UnauthorizedAccessException | Η διαδρομή καθόρισε έναν φάκελο. -ή- Ο καλών δεν διαθέτει την απαιτούμενη άδεια. |

## Παραδείγματα

Αυτό το παράδειγμα εξάγει σε έναν φάκελο ένα αρχείο με τρία τμήματα.

```csharp
using (Archive a = new Archive("archive.zip", new string[] { "archive.z01", "archive.z02" }))
{
    a.ExtractToDirectory("destination");
}
```

### Δείτε επίσης

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


