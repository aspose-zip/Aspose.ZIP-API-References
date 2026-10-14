---
title: "SevenZipArchive.SevenZipArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής SevenZipArchive. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης SevenZipArchive με προαιρετικές ρυθμίσεις για τις καταχωρήσεις της"
type: docs
weight: 10
url: /el/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`SevenZipArchive`](../) με προαιρετικές ρυθμίσεις για τις καταχωρήσεις της.

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για τα πρόσφατα προστιθέμενα στοιχεία [`SevenZipArchiveEntry`](../../sevenziparchiveentry/). Εάν δεν καθοριστούν, θα χρησιμοποιηθεί συμπίεση LZMA χωρίς κρυπτογράφηση. |

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα μόνο αρχείο με τις προεπιλεγμένες ρυθμίσεις: συμπίεση LZMA χωρίς κρυπτογράφηση.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Δείτε επίσης

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream, string) {#constructor_2}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`SevenZipArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από την αρχειοθήκη.

```csharp
public SevenZipArchive(Stream sourceStream, string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| password | String | Προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση. Εάν τα ονόματα αρχείων είναι κρυπτογραφημένα, πρέπει να υπάρχει. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *sourceStream* δεν είναι δυνατόν να γίνει αναζήτηση. |
| ArgumentNullException | *sourceStream* είναι null. |
| NotImplementedException | Το αρχείο περιέχει περισσότερους από έναν κωδικοποιητή. Τώρα υποστηρίζεται μόνο η συμπίεση LZMA. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`ExtractToDirectory`](../extracttodirectory/) για αποσυμπίεση.

## Παραδείγματα

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(string, string) {#constructor_4}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`SevenZipArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από την αρχειοθήκη.

```csharp
public SevenZipArchive(string path, string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η πλήρης ή σχετική διαδρομή προς το αρχείο του αρχείου. |
| password | String | Προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση. Εάν τα ονόματα αρχείων είναι κρυπτογραφημένα, πρέπει να υπάρχει. |

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

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`ExtractToDirectory`](../extracttodirectory/) για αποσυμπίεση.

## Παραδείγματα

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream, SevenZipLoadOptions) {#constructor_1}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`SevenZipArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από την αρχειοθήκη.

```csharp
public SevenZipArchive(Stream sourceStream, SevenZipLoadOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| επιλογές | SevenZipLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *sourceStream* δεν είναι δυνατόν να γίνει αναζήτηση. |
| ArgumentNullException | *sourceStream* είναι null. |
| NotImplementedException | Το αρχείο περιέχει περισσότερους από έναν κωδικοποιητή. Τώρα υποστηρίζεται μόνο η συμπίεση LZMA. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`ExtractToDirectory`](../extracttodirectory/) για αποσυμπίεση.

## Παραδείγματα

Αποσυμπιέστε ένα κρυπτογραφημένο αρχείο. Επιτρέψτε έως 60 δευτερόλεπτα για την εκτέλεση, ακυρώστε μετά από αυτή τη διάρκεια.

```csharp
using(CancellationTokenSource cts = new CancellationTokenSource())
{
    SevenZipLoadOptions options = new SevenZipLoadOptions(){ DecryptionPassword = "Top$ecr3t", CancellationToken = cts.Token }
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z"), options))
    {
        archive.ExtractToDirectory("C:\\extracted");
    }
}
```

### Δείτε επίσης

* class [SevenZipLoadOptions](../../sevenziploadoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(string, SevenZipLoadOptions) {#constructor_3}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`SevenZipArchive`](../) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από την αρχειοθήκη.

```csharp
public SevenZipArchive(string path, SevenZipLoadOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η πλήρης ή σχετική διαδρομή προς το αρχείο του αρχείου. |
| επιλογές | SevenZipLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

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

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [`ExtractToDirectory`](../extracttodirectory/) για αποσυμπίεση.

## Παραδείγματα

Αποσυμπιέστε ένα κρυπτογραφημένο αρχείο. Επιτρέψτε έως 60 δευτερόλεπτα για την εκτέλεση, ακυρώστε μετά από αυτή τη διάρκεια.

```csharp
using(CancellationTokenSource cts = new CancellationTokenSource())
{
    SevenZipLoadOptions options = new SevenZipLoadOptions(){ DecryptionPassword = "Top$ecr3t", CancellationToken = cts.Token }
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z"), options))
    {
        archive.ExtractToDirectory("C:\\extracted");
    }
}
```

### Δείτε επίσης

* class [SevenZipLoadOptions](../../sevenziploadoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(string[], string) {#constructor_5}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`SevenZipArchive`](../) από αρχείο 7z πολλαπλών τόμων και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

```csharp
public SevenZipArchive(string[] parts, string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| parts | String[] | Διαδρομές για κάθε τμήμα του αρχείου 7z πολλαπλών τόμων, τηρώντας τη σειρά |
| password | String | Προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση. Εάν τα ονόματα αρχείων είναι κρυπτογραφημένα, πρέπει να υπάρχει. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *parts* είναι null. |
| ArgumentException | *parts* δεν έχει καταχωρήσεις. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η διαδρομή προς ένα αρχείο είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση σε ένα αρχείο απορρίπτεται. |
| PathTooLongException | Η καθορισμένη διαδρομή προς ένα τμήμα, το όνομα αρχείου ή και τα δύο υπερβαίνει το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο σε μια διαδρομή περιέχει άνω-κάτω τελεία (:) στη μέση της συμβολοσειράς. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |

## Παραδείγματα

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new string[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" }))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


