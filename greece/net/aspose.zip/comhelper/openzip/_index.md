---
title: "ComHelper.OpenZip"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος ComHelper. Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα ZIP από ένα stream"
type: docs
weight: 50
url: /el/net/aspose.zip/comhelper/openzip/
---
## OpenZip(Stream) {#openzip}

Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο ZIP από μια ροή.

```csharp
public Archive OpenZip(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Ένα αντικείμενο ροής .NET που περιέχει το αρχείο προς φόρτωση. |

### Τιμή Επιστροφής

Ένα αντικείμενο [`Archive`](../../archive/) που αντιπροσωπεύει το αρχείο.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |

### Δείτε επίσης

* class [Archive](../../archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenZip(string) {#openzip_1}

Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο ZIP από ένα αρχείο.

```csharp
public Archive OpenZip(string fileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Όνομα αρχείου του αρχείου προς φόρτωση. |

### Τιμή Επιστροφής

Ένα αντικείμενο [`Archive`](../../archive/) που αντιπροσωπεύει το αρχείο.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| ArgumentException | Το όνομα αρχείου είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| ArgumentNullException | *fileName* είναι `null`. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. |
| UnauthorizedAccessException | Η πρόσβαση στο *fileName* απορρίπτεται. |

### Δείτε επίσης

* class [Archive](../../archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


