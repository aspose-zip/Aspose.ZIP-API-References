---
title: "AppleArchive.CreateEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος AppleArchive. Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο"
type: docs
weight: 60
url: /el/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| διαδρομή | String | Η διαδρομή του αρχείου προς συμπίεση. |
| openImmediately | Boolean | True, εάν το αρχείο ανοίξει αμέσως, διαφορετικά το αρχείο ανοίγει κατά την αποθήκευση του αρχείου. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Apple Archive.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί. |
| ArgumentException | *name* είναι κενό. |
| ArgumentNullException | *path* είναι `null`. |

### Δείτε επίσης

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| source | Stream | Η ροή εισόδου για την καταχώρηση. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Apple Archive.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί. |
| ArgumentException | *name* είναι κενό. |
| ArgumentNullException | *source* είναι `null`. |

### Δείτε επίσης

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της καταχώρησης. |
| fileInfo | FileInfo | Τα μεταδεδομένα του αρχείου που θα συμπιεστεί. |
| openImmediately | Boolean | True, εάν το αρχείο ανοίξει αμέσως, διαφορετικά το αρχείο ανοίγει κατά την αποθήκευση του αρχείου. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Apple Archive.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί. |
| ArgumentException | *name* είναι κενό. |
| ArgumentNullException | *fileInfo* είναι `null`. |

### Δείτε επίσης

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


