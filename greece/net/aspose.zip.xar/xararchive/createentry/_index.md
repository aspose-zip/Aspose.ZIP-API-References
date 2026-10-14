---
title: "XarArchive.CreateEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος XarArchive. Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο"
type: docs
weight: 40
url: /el/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| fileInfo | FileInfo | Τα μεταδεδομένα του αρχείου ή φακέλου που θα συμπιεστεί. |
| openImmediately | Boolean | True, εάν το αρχείο ανοίξει αμέσως, διαφορετικά το αρχείο ανοίγει κατά την αποθήκευση του αρχείου. |
| compressionSettings | XarCompressionSettings | Οι ρυθμίσεις συμπίεσης που χρησιμοποιούνται για το προστεθέν στοιχείο [`XarEntry`](../../xarentry/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Xar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *name* είναι null. |
| ArgumentException | *name* είναι κενό. |
| ArgumentNullException | *fileInfo* είναι null. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παρατηρήσεις

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο *openImmediately*, θα παραμείνει κλειδωμένο μέχρι να απελευθερωθεί το αρχείο.

## Παραδείγματα

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### Δείτε επίσης

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| sourcePath | String | Διαδρομή προς το αρχείο που θα συμπιεστεί. |
| openImmediately | Boolean | True, εάν το αρχείο ανοίξει αμέσως, διαφορετικά το αρχείο ανοίγει κατά την αποθήκευση του αρχείου. |
| compressionSettings | XarCompressionSettings | Οι ρυθμίσεις συμπίεσης που χρησιμοποιούνται για το προστεθέν στοιχείο [`XarEntry`](../../xarentry/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Xar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *sourcePath* είναι null. |
| SecurityException | Το πρόγραμμα που καλεί δεν διαθέτει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | Το *sourcePath* είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει άκυρους χαρακτήρες. - ή - Το όνομα αρχείου, ως μέρος του *name*, υπερβαίνει τα 100 σύμβολα. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *sourcePath* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο *sourcePath*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. - ή - *name* είναι πολύ μεγάλο για xar. |
| NotSupportedException | Το αρχείο στο *sourcePath* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |
| InvalidOperationException | Αδύνατη η τροποποίηση του αρχείου xar. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παρατηρήσεις

Το όνομα της καταχώρησης ορίζεται αποκλειστικά από την παράμετρο *name*. Το όνομα αρχείου που παρέχεται στην παράμετρο *sourcePath* δεν επηρεάζει το όνομα της καταχώρησης.

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο *openImmediately*, θα παραμείνει κλειδωμένο μέχρι να απελευθερωθεί το αρχείο.

## Παραδείγματα

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### Δείτε επίσης

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

Δημιουργεί μια μοναδική καταχώρηση μέσα στην αρχειοθήκη.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |
| compressionSettings | XarCompressionSettings | Οι ρυθμίσεις συμπίεσης που χρησιμοποιούνται για το προστεθέν στοιχείο [`XarEntry`](../../xarentry/). |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Xar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *name* είναι null. |
| ArgumentNullException | *source* είναι null. |
| ArgumentException | *name* είναι κενό. |
| InvalidOperationException | Αδύνατη η τροποποίηση του αρχείου xar. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### Δείτε επίσης

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


