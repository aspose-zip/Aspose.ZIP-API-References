---
title: "SevenZipArchive.CreateEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος SevenZipArchive. Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη"
type: docs
weight: 50
url: /el/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry_1}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| fileInfo | FileInfo | Τα μεταδεδομένα του αρχείου που θα συμπιεστεί. |
| openImmediately | Boolean | True, εάν το αρχείο ανοίξει αμέσως, διαφορετικά το αρχείο ανοίγει κατά την αποθήκευση του αρχείου. |
| newEntrySettings | SevenZipEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`SevenZipArchiveEntry`](../../sevenziparchiveentry/). Οι ατομικές ρυθμίσεις συμπίεσης αγνοούνται σε περίπτωση συμπαγούς συμπίεσης, δείτε [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |

### Τιμή Επιστροφής

Παράδειγμα αντικειμένου Seven Zip.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* είναι μόνο για ανάγνωση ή είναι ένας φάκελος. |
| ArgumentException | Το *name* είναι null ή κενό. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *fileInfo* δεν επηρεάζει το όνομα της καταχώρησης.

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο *openImmediately*, θα παραμείνει κλειδωμένο μέχρι να αποθηκευτεί το αρχείο.

## Παραδείγματα

Δημιουργήστε μια αρχειοθήκη με καταχωρήσεις κρυπτογραφημένες με διαφορετικούς κωδικούς πρόσβασης.

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
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_3}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |
| newEntrySettings | SevenZipEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`SevenZipArchiveEntry`](../../sevenziparchiveentry/). Οι ατομικές ρυθμίσεις συμπίεσης αγνοούνται σε περίπτωση συμπαγούς συμπίεσης, δείτε [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |
| fileInfo | FileSystemInfo | Τα μεταδεδομένα του αρχείου ή φακέλου που θα συμπιεστεί. |

### Τιμή Επιστροφής

Παράδειγμα αντικειμένου SevenZip.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Τόσο *source* όσο και *fileInfo* είναι `null` ή *source* είναι `null` και *fileInfo* αντιπροσωπεύει φάκελο. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentException | Το *name* είναι null ή κενό. |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *fileInfo* δεν επηρεάζει το όνομα της καταχώρησης.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## Παραδείγματα

Δημιουργήστε μια αρχειοθήκη με καταχώρηση κρυπτογραφημένη και συμπιεσμένη με LZMA2.

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
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, SevenZipEntrySettings) {#createentry}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Func<Stream> streamProvider, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| streamProvider | Func`1 | Η μέθοδος που παρέχει ροή εισόδου για την καταχώρηση. |
| newEntrySettings | SevenZipEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`SevenZipArchiveEntry`](../../sevenziparchiveentry/). Οι ατομικές ρυθμίσεις συμπίεσης αγνοούνται σε περίπτωση συμπαγούς συμπίεσης, δείτε [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |

### Τιμή Επιστροφής

Παράδειγμα αντικειμένου SevenZip.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Η αρχειοθήκη δημιουργείται για αποσυμπίεση |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentException | Το *name* είναι null ή κενό. |

## Παραδείγματα

Δημιουργήστε μια αρχειοθήκη με καταχώρηση κρυπτογραφημένη και συμπιεσμένη με LZMA2.

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1"))); 
        archive.Save(sevenZipFile);
    }
}
```

### Δείτε επίσης

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_2}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |
| newEntrySettings | SevenZipEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`SevenZipArchiveEntry`](../../sevenziparchiveentry/). Οι ατομικές ρυθμίσεις συμπίεσης αγνοούνται σε περίπτωση συμπαγούς συμπίεσης, δείτε [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Zip.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentException | Το *name* είναι null ή κενό. |

## Παραδείγματα

Δημιουργήστε μια αρχειοθήκη 7z με συμπίεση LZMA2 και κρυπτογράφηση όλων των καταχωρήσεων.

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
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_4}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| διαδρομή | String | Το πλήρως προσδιορισμένο όνομα του νέου αρχείου, ή το σχετικό όνομα αρχείου που θα συμπιεστεί. |
| openImmediately | Boolean | True, εάν το αρχείο ανοίξει αμέσως, διαφορετικά το αρχείο ανοίγει κατά την αποθήκευση του αρχείου. |
| newEntrySettings | SevenZipEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`SevenZipArchiveEntry`](../../sevenziparchiveentry/). Οι ατομικές ρυθμίσεις συμπίεσης αγνοούνται σε περίπτωση συμπαγούς συμπίεσης, δείτε [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Zip.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Το *path* είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. - ή - Το *name* είναι null ή κενό. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *path* δεν επηρεάζει το όνομα της καταχώρησης.

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο *openImmediately*, θα παραμείνει κλειδωμένο μέχρι να αποθηκευτεί το αρχείο.

## Παραδείγματα

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
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


