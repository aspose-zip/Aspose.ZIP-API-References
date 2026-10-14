---
title: "ComHelper.OpenRar"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος ComHelper. Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα rar αρχείο από μια ροή."
type: docs
weight: 40
url: /el/net/aspose.zip/comhelper/openrar/
---
## OpenRar(Stream) {#openrar}

Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο rar από μια ροή.

```csharp
public RarArchive OpenRar(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Ένα αντικείμενο ροής .NET που περιέχει το αρχείο προς φόρτωση. |

### Τιμή Επιστροφής

Ένα αντικείμενο [`RarArchive`](../../../aspose.zip.rar/rararchive/) που αντιπροσωπεύει το αρχείο.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidDataException | Εκτοπίζεται όταν τα δεδομένα είναι μη έγκυρα ή κατεστραμμένα. |

### Δείτε επίσης

* class [RarArchive](../../../aspose.zip.rar/rararchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenRar(string) {#openrar_1}

Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο rar από ένα αρχείο.

```csharp
public RarArchive OpenRar(string fileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Όνομα αρχείου του αρχείου προς φόρτωση. |

### Τιμή Επιστροφής

Ένα αντικείμενο [`RarArchive`](../../../aspose.zip.rar/rararchive/) που αντιπροσωπεύει το αρχείο.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | Το όνομα αρχείου είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| ArgumentNullException | *fileName* είναι `null`. |
| Εξαίρεση | Εκτοξεύεται όταν συμβαίνει σφάλμα χρόνου εκτέλεσης. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| InvalidDataException | Εκτοπίζεται όταν τα δεδομένα είναι μη έγκυρα ή κατεστραμμένα. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. |
| UnauthorizedAccessException | Η πρόσβαση στο *fileName* απορρίπτεται. |

### Δείτε επίσης

* class [RarArchive](../../../aspose.zip.rar/rararchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


