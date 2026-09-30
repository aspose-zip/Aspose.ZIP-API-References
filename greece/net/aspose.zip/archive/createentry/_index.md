---
title: "Archive.CreateEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος Archive. Δημιουργεί μία μοναδική καταχώρηση μέσα στο αρχείο"
type: docs
weight: 60
url: /el/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_4}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| διαδρομή | String | Το πλήρως προσδιορισμένο όνομα του νέου αρχείου, ή το σχετικό όνομα αρχείου που θα συμπιεστεί. |
| openImmediately | Boolean | True, εάν το αρχείο ανοίξει αμέσως, διαφορετικά το αρχείο ανοίγει κατά την αποθήκευση του αρχείου. |
| newEntrySettings | ArchiveEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`ArchiveEntry`](../../archiveentry/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Zip.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| ObjectDisposedException | Εκτοπίζεται εάν το αρχείο έχει διαγραφεί. |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *path* δεν επηρεάζει το όνομα της καταχώρησης.

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο *openImmediately*, θα παραμείνει κλειδωμένο μέχρι να αποθηκευτεί το αρχείο.

## Παραδείγματα

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

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_2}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |
| newEntrySettings | ArchiveEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`ArchiveEntry`](../../archiveentry/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Zip.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Εκτοπίζεται εάν το αρχείο έχει διαγραφεί. |
| InvalidOperationException | Εκτοξεύεται όταν η προσθήκη της καταχώρησης δεν είναι έγκυρη λόγω της τρέχουσας κατάστασης του αρχείου. |

## Παραδείγματα

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### Δείτε επίσης

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry_1}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| fileInfo | FileInfo | Τα μεταδεδομένα του αρχείου που θα συμπιεστεί. |
| openImmediately | Boolean | True, εάν το αρχείο ανοίξει αμέσως, διαφορετικά το αρχείο ανοίγει κατά την αποθήκευση του αρχείου. |
| newEntrySettings | ArchiveEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`ArchiveEntry`](../../archiveentry/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Zip.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* είναι μόνο για ανάγνωση ή είναι ένας φάκελος. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |
| ObjectDisposedException | Εκτοπίζεται εάν το αρχείο έχει διαγραφεί. |
| InvalidOperationException | Εκτοξεύεται όταν η προσθήκη της καταχώρησης δεν είναι έγκυρη λόγω της τρέχουσας κατάστασης του αρχείου. |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *fileInfo* δεν επηρεάζει το όνομα της καταχώρησης.

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο *openImmediately*, θα παραμείνει κλειδωμένο μέχρι να αποθηκευτεί το αρχείο.

## Παραδείγματα

Δημιουργήστε αρχείο με καταχωρήσεις κρυπτογραφημένες με διαφορετικές μεθόδους κρυπτογράφησης και κωδικούς πρόσβασης για κάθε μία.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### Δείτε επίσης

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_3}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |
| newEntrySettings | ArchiveEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`ArchiveEntry`](../../archiveentry/). |
| fileInfo | FileSystemInfo | Τα μεταδεδομένα του αρχείου ή φακέλου που θα συμπιεστεί. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Zip.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Τόσο *source* όσο και *fileInfo* είναι `null` ή *source* είναι `null` και *fileInfo* αντιπροσωπεύει φάκελο. |
| ObjectDisposedException | Εκτοπίζεται εάν το αρχείο έχει διαγραφεί. |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *fileInfo* δεν επηρεάζει το όνομα της καταχώρησης.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## Παραδείγματα

Δημιουργήστε αρχείο με κρυπτογραφημένη καταχώρηση.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### Δείτε επίσης

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, ArchiveEntrySettings) {#createentry}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public ArchiveEntry CreateEntry(string name, Func<Stream> streamProvider, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| streamProvider | Func`1 | Η μέθοδος που παρέχει ροή εισόδου για την καταχώρηση. |
| newEntrySettings | ArchiveEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`ArchiveEntry`](../../archiveentry/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Zip.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Εκτοπίζεται εάν το αρχείο έχει διαγραφεί. |
| ArgumentException | Εκτοπίζεται όταν το *name* είναι `null` ή κενό, ή το *streamProvider* είναι `null`. |
| InvalidOperationException | Εκτοπίζεται όταν το αρχείο δεν υποστηρίζει προσθήκη καταχώρησης. |

## Παρατηρήσεις

Αυτή η μέθοδος είναι για .NET Framework 4.0 και νεότερο, καθώς και για .NET Standard 2.0 και νεότερη έκδοση.

## Παραδείγματα

Δημιουργήστε αρχείο με κρυπτογραφημένη καταχώρηση.

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")))); 
        archive.Save(zipFile);
    }
}
```

### Δείτε επίσης

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


