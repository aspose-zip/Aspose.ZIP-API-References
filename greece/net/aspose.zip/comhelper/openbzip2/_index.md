---
title: "ComHelper.OpenBzip2"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος ComHelper. Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα bzip2 αρχείο από μια ροή."
type: docs
weight: 20
url: /el/net/aspose.zip/comhelper/openbzip2/
---
## OpenBzip2(Stream) {#openbzip2}

Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο bzip2 από ροή.

```csharp
public Bzip2Archive OpenBzip2(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Ένα αντικείμενο ροής .NET που περιέχει το αρχείο προς φόρτωση. |

### Τιμή Επιστροφής

Ένα αντικείμενο [`Bzip2Archive`](../../../aspose.zip.bzip2/bzip2archive/) που αντιπροσωπεύει το αρχείο.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| InvalidDataException | Λάθος bytes υπογραφής. |

### Δείτε επίσης

* class [Bzip2Archive](../../../aspose.zip.bzip2/bzip2archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenBzip2(string) {#openbzip2_1}

Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο bzip2 από αρχείο.

```csharp
public Bzip2Archive OpenBzip2(string fileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Όνομα αρχείου του αρχείου προς φόρτωση. |

### Τιμή Επιστροφής

Ένα αντικείμενο [`Bzip2Archive`](../../../aspose.zip.bzip2/bzip2archive/) που αντιπροσωπεύει το αρχείο.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| ArgumentException | Το όνομα αρχείου είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| ArgumentNullException | *fileName* είναι `null`. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| InvalidDataException | Λάθος bytes υπογραφής. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. |
| UnauthorizedAccessException | Η πρόσβαση στο *fileName* απορρίπτεται. |

### Δείτε επίσης

* class [Bzip2Archive](../../../aspose.zip.bzip2/bzip2archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


