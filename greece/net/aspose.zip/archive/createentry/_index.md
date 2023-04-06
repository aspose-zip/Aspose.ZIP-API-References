---
title: Archive.CreateEntry
second_title: Aspose.ZIP για Αναφορά API .NET
description: Archive μέθοδος. Δημιουργία μίας καταχώρησης μέσα στο αρχείο.
type: docs
weight: 50
url: /el/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| path | String | Το πλήρως αναγνωρισμένο όνομα του νέου αρχείου ή το σχετικό όνομα αρχείου που πρόκειται να συμπιεστεί. |
| openImmediately | Boolean | Σωστό εάν ανοίξετε το αρχείο αμέσως, διαφορετικά ανοίξτε το αρχείο κατά την αποθήκευση αρχειοθέτησης. |
| newEntrySettings | ArchiveEntrySettings | Προστέθηκαν ρυθμίσεις συμπίεσης και κρυπτογράφησης[`ArchiveEntry`](../../archiveentry/) είδος. |

### Επιστρεφόμενη Αξία

Περίπτωση εισόδου zip.

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

Το όνομα καταχώρισης ορίζεται αποκλειστικά μέσα*name* παράμετρος. Το όνομα αρχείου που παρέχεται*path* η παράμετρος δεν επηρεάζει το όνομα της καταχώρισης.

Εάν το αρχείο ανοίξει αμέσως με*openImmediately* η παράμετρος αποκλείεται μέχρι να αποθηκευτεί το αρχείο.

### Παραδείγματα

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
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |
| newEntrySettings | ArchiveEntrySettings | Προστέθηκαν ρυθμίσεις συμπίεσης και κρυπτογράφησης[`ArchiveEntry`](../../archiveentry/) είδος. |

### Επιστρεφόμενη Αξία

Περίπτωση εισόδου zip.

### Παραδείγματα

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
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| fileInfo | FileInfo | Τα μεταδεδομένα του αρχείου που πρόκειται να συμπιεστούν. |
| openImmediately | Boolean | Σωστό εάν ανοίξετε το αρχείο αμέσως, διαφορετικά ανοίξτε το αρχείο κατά την αποθήκευση αρχειοθέτησης. |
| newEntrySettings | ArchiveEntrySettings | Προστέθηκαν ρυθμίσεις συμπίεσης και κρυπτογράφησης[`ArchiveEntry`](../../archiveentry/) είδος. |

### Επιστρεφόμενη Αξία

Περίπτωση εισόδου zip.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* είναι μόνο για ανάγνωση ή είναι κατάλογος. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή δεν είναι έγκυρη, όπως είναι σε μη αντιστοιχισμένη μονάδα δίσκου. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |

### Παρατηρήσεις

Το όνομα καταχώρισης ορίζεται αποκλειστικά μέσα*name* παράμετρος. Το όνομα αρχείου που παρέχεται*fileInfo* η παράμετρος δεν επηρεάζει το όνομα της καταχώρισης.

Εάν το αρχείο ανοίξει αμέσως με*openImmediately* η παράμετρος αποκλείεται μέχρι να αποθηκευτεί το αρχείο.

### Παραδείγματα

Σύνθεση αρχείου με καταχωρήσεις κρυπτογραφημένες με διαφορετικές μεθόδους κρυπτογράφησης και κωδικούς πρόσβασης το καθένα.

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
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |
| newEntrySettings | ArchiveEntrySettings | Προστέθηκαν ρυθμίσεις συμπίεσης και κρυπτογράφησης[`ArchiveEntry`](../../archiveentry/) είδος. |
| fileInfo | FileSystemInfo | Τα μεταδεδομένα του αρχείου ή του φακέλου που πρόκειται να συμπιεστούν. |

### Επιστρεφόμενη Αξία

Περίπτωση εισόδου zip.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| InvalidOperationException | Και τα δυο*source* και*fileInfo* είναι μηδενικά ή*source*είναι μηδενικό και*fileInfo* σημαίνει κατάλογος. |

### Παρατηρήσεις

Το όνομα καταχώρισης ορίζεται αποκλειστικά μέσα*name* παράμετρος. Το όνομα αρχείου που παρέχεται*fileInfo* η παράμετρος δεν επηρεάζει το όνομα της καταχώρισης.

*fileInfo* μπορεί να αναφέρεται σεDirectoryInfo εάν η καταχώρηση είναι κατάλογος.

### Παραδείγματα

Σύνθεση αρχείου με κρυπτογραφημένη καταχώρηση.

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
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)


