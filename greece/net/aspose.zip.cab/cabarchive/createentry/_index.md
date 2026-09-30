---
title: "CabArchive.CreateEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος CabArchive. Δημιουργήστε μία ενιαία καταχώρηση μέσα στο αρχείο"
type: docs
weight: 40
url: /el/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| διαδρομή | String | Το πλήρως προσδιορισμένο όνομα του νέου αρχείου, ή το σχετικό όνομα αρχείου που θα συμπιεστεί. |
| newEntrySettings | CabEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`CabEntry`](../../cabentry/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Cab.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για εξαγωγή και δεν μπορεί να προσθέσει καταχωρήσεις. |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *path* δεν επηρεάζει το όνομα της καταχώρησης.

## Παραδείγματα

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### Δείτε επίσης

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |
| newEntrySettings | CabEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`CabEntry`](../../cabentry/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Cab.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για εξαγωγή και δεν μπορεί να προσθέσει καταχωρήσεις. |
| ArgumentNullException | *name* είναι null. |

## Παραδείγματα

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### Δείτε επίσης

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| fileInfo | FileInfo | Τα μεταδεδομένα του αρχείου που θα συμπιεστεί. |
| newEntrySettings | CabEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`CabEntry`](../../cabentry/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης CAB.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* είναι μόνο για ανάγνωση ή είναι ένας φάκελος. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |
| FileNotFoundException | *fileInfo* αντιπροσωπεύει ένα αρχείο που δεν μπορεί να βρεθεί. |
| SecurityException | Ο καλών δεν διαθέτει την απαιτούμενη άδεια για πρόσβαση στο *fileInfo*. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για εξαγωγή και δεν μπορεί να προσθέσει καταχωρήσεις. |
| ArgumentNullException | *name* είναι null. |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *fileInfo* δεν επηρεάζει το όνομα της καταχώρησης.

## Παραδείγματα

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### Δείτε επίσης

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| streamProvider | Func`1 | Η μέθοδος που παρέχει ροή εισόδου για την καταχώρηση. |
| newEntrySettings | CabEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [`CabEntry`](../../cabentry/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης CAB.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Το αρχείο δημιουργείται για αποσυμπίεση. - ή - Ο αριθμός των αρχείων έχει φτάσει το όριο. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentException | Το *name* είναι null ή κενό. |

## Παραδείγματα

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### Δείτε επίσης

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


