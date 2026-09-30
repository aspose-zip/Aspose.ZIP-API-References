---
title: "ArchiveFactory.GetArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος ArchiveFactory. Ανιχνεύει τη μορφή του αρχείου και δημιουργεί το κατάλληλο αντικείμενο IArchive σύμφωνα με τον τύπο του αρχείου που καθορίζεται από το δοσμένο μονοπάτι."
type: docs
weight: 20
url: /el/net/aspose.zip/archivefactory/getarchive/
---
## GetArchive(string) {#getarchive_2}

Ανιχνεύει τη μορφή του αρχείου και δημιουργεί το κατάλληλο αντικείμενο [`IArchive`](../../iarchive/) σύμφωνα με τον τύπο του αρχείου που καθορίζεται από το δοσμένο μονοπάτι.

```csharp
public static IArchive GetArchive(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Το μονοπάτι προς το αρχείο που θα αναλυθεί. |

### Τιμή Επιστροφής

Ένα αντικείμενο [`IArchive`](../../iarchive/) που αντιπροσωπεύει το αρχείο.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι `null`. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη (για παράδειγμα, βρίσκεται σε μη αντιστοιχισμένο δίσκο). |
| FileNotFoundException | Το αρχείο που καθορίστηκε στο *path* δεν βρέθηκε. |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά το άνοιγμα του αρχείου. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. |
| UnauthorizedAccessException | *path* καθόρισε έναν φάκελο. -ή- Ο καλών δεν έχει τα απαιτούμενα δικαιώματα. |

### Δείτε επίσης

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)

---

## GetArchive(Stream) {#getarchive}

Ανιχνεύει τη μορφή του αρχείου και δημιουργεί το κατάλληλο αντικείμενο [`IArchive`](../../iarchive/) σύμφωνα με τον τύπο του αρχείου που καθορίζεται από το δοσμένο stream.

```csharp
public static IArchive GetArchive(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Το stream που περιέχει τα δεδομένα του αρχείου. Πρέπει να είναι αναζητήσιμο. |

### Τιμή Επιστροφής

Ένα αντικείμενο [`IArchive`](../../iarchive/) που αντιπροσωπεύει το αρχείο.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *stream* δεν είναι δυνατόν να γίνει αναζήτηση. |
| ArgumentNullException | *stream* είναι null. |

### Δείτε επίσης

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)

---

## GetArchive(Stream, string) {#getarchive_1}

Ανιχνεύει τη μορφή του αρχείου και δημιουργεί το κατάλληλο αντικείμενο [`IArchive`](../../iarchive/) σύμφωνα με τον τύπο του κρυπτογραφημένου αρχείου που καθορίζεται από το δοσμένο stream.

```csharp
public static IArchive GetArchive(Stream stream, string password)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Το stream που περιέχει τα δεδομένα του αρχείου. Πρέπει να είναι αναζητήσιμο. |
| password | String | Κωδικός πρόσβασης για την αποκρυπτογράφηση ενός κρυπτογραφημένου αρχείου. |

### Τιμή Επιστροφής

Ένα αντικείμενο [`IArchive`](../../iarchive/) που αντιπροσωπεύει το αρχείο.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *stream* δεν είναι δυνατόν να γίνει αναζήτηση. |
| ArgumentNullException | *stream* είναι null. |

### Δείτε επίσης

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


