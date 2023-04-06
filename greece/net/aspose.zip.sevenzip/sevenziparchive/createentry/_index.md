---
title: SevenZipArchive.CreateEntry
second_title: Aspose.ZIP για Αναφορά API .NET
description: SevenZipArchive μέθοδος. Δημιουργία μίας καταχώρησης μέσα στο αρχείο.
type: docs
weight: 50
url: /el/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| fileInfo | FileInfo | Τα μεταδεδομένα του αρχείου που πρόκειται να συμπιεστούν. |
| openImmediately | Boolean | Σωστό εάν ανοίξετε το αρχείο αμέσως, διαφορετικά ανοίξτε το αρχείο κατά την αποθήκευση αρχειοθέτησης. |
| newEntrySettings | SevenZipEntrySettings | Προστέθηκαν ρυθμίσεις συμπίεσης και κρυπτογράφησης[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) είδος. |

### Επιστρεφόμενη Αξία

Περίπτωση εισόδου επτά Zip.

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

Σύνθεση αρχείου με καταχωρήσεις κρυπτογραφημένες με διαφορετικούς κωδικούς πρόσβασης η καθεμία.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### Δείτε επίσης

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |
| newEntrySettings | SevenZipEntrySettings | Προστέθηκαν ρυθμίσεις συμπίεσης και κρυπτογράφησης[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) είδος. |
| fileInfo | FileSystemInfo | Τα μεταδεδομένα του αρχείου ή του φακέλου που πρόκειται να συμπιεστούν. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής SevenZip.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| InvalidOperationException | Και τα δυο*source* και*fileInfo* είναι μηδενικά ή*source*είναι μηδενικό και*fileInfo* σημαίνει κατάλογος. |

### Παρατηρήσεις

Το όνομα καταχώρισης ορίζεται αποκλειστικά μέσα*name* παράμετρος. Το όνομα αρχείου που παρέχεται*fileInfo* η παράμετρος δεν επηρεάζει το όνομα της καταχώρισης.

*fileInfo* μπορεί να αναφέρεται σεDirectoryInfo εάν η καταχώρηση είναι κατάλογος.

### Παραδείγματα

Σύνθεση αρχείου με συμπιεσμένη κρυπτογραφημένη καταχώρηση LZMA2.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### Δείτε επίσης

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |
| newEntrySettings | SevenZipEntrySettings | Προστέθηκαν ρυθμίσεις συμπίεσης και κρυπτογράφησης[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) είδος. |

### Επιστρεφόμενη Αξία

Περίπτωση εισόδου zip.

### Παραδείγματα

Σύνθεση αρχείου 7z με συμπίεση LZMA2 και κρυπτογράφηση όλων των καταχωρήσεων.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### Δείτε επίσης

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

Δημιουργία μίας καταχώρησης μέσα στο αρχείο.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρισης. |
| path | String | Το πλήρως αναγνωρισμένο όνομα του νέου αρχείου ή το σχετικό όνομα αρχείου που πρόκειται να συμπιεστεί. |
| openImmediately | Boolean | Σωστό εάν ανοίξετε το αρχείο αμέσως, διαφορετικά ανοίξτε το αρχείο κατά την αποθήκευση αρχειοθέτησης. |
| newEntrySettings | SevenZipEntrySettings | Προστέθηκαν ρυθμίσεις συμπίεσης και κρυπτογράφησης[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) είδος. |

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
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Δείτε επίσης

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)


