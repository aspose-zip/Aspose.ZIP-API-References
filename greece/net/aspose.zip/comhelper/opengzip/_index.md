---
title: "ComHelper.OpenGzip"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος ComHelper. Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα gzip αρχείο από μια ροή"
type: docs
weight: 30
url: /el/net/aspose.zip/comhelper/opengzip/
---
## OpenGzip(Stream) {#opengzip}

Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο gzip από ροή.

```csharp
public GzipArchive OpenGzip(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Ένα αντικείμενο ροής .NET που περιέχει το αρχείο προς φόρτωση. |

### Τιμή Επιστροφής

Ένα αντικείμενο [`GzipArchive`](../../../aspose.zip.gzip/gziparchive/) που αντιπροσωπεύει το αρχείο.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| ArgumentNullException | Εκτοπίζεται όταν ένα *stream* είναι null. |
| InvalidDataException | Εκτοπίζεται όταν τα δεδομένα είναι μη έγκυρα ή κατεστραμμένα. |

### Δείτε επίσης

* class [GzipArchive](../../../aspose.zip.gzip/gziparchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenGzip(string) {#opengzip_1}

Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο gzip από ένα αρχείο.

```csharp
public GzipArchive OpenGzip(string fileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Όνομα αρχείου του αρχείου προς φόρτωση. |

### Τιμή Επιστροφής

Ένα αντικείμενο [`GzipArchive`](../../../aspose.zip.gzip/gziparchive/) που αντιπροσωπεύει το αρχείο.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| ArgumentException | Το όνομα αρχείου είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| ArgumentNullException | *fileName* είναι `null`. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| InvalidDataException | Εκτοπίζεται όταν τα δεδομένα είναι μη έγκυρα ή κατεστραμμένα. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. |
| UnauthorizedAccessException | Η πρόσβαση στο *fileName* απορρίπτεται. |

### Δείτε επίσης

* class [GzipArchive](../../../aspose.zip.gzip/gziparchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


