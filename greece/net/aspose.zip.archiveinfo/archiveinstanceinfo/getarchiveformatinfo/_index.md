---
title: ArchiveInstanceInfo.GetArchiveFormatInfo
second_title: Aspose.ZIP για Αναφορά API .NET
description: ArchiveInstanceInfo μέθοδος. Λαμβάνει πληροφορίες μορφής αρχείου.
type: docs
weight: 50
url: /el/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveformatinfo/
---
## GetArchiveFormatInfo(string) {#getarchiveformatinfo_1}

Λαμβάνει πληροφορίες μορφής αρχείου.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(string fileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Το όνομα αρχείου του αρχείου αρχειοθέτησης. |

### Επιστρεφόμενη Αξία

Πληροφορίες σχετικά με τη μορφή αρχειοθέτησης ή μηδενική αν δεν εντοπίστηκε η μορφή.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *fileName* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*fileName* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*fileName* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*fileName* υπερβαίνει το καθορισμένο από το σύστημα μέγιστο μήκος. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*fileName* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά το άνοιγμα του αρχείου. |

### Δείτε επίσης

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* χώρος ονομάτων [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* συνέλευση [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

Λαμβάνει πληροφορίες μορφής αρχείου.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή του αρχείου αρχείου. |

### Επιστρεφόμενη Αξία

Πληροφορίες σχετικά με τη μορφή αρχειοθέτησης ή μηδενική αν δεν εντοπίστηκε η μορφή.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *stream* είναι μηδενικό. |
| ArgumentException | *stream* δεν είναι αναζητήσιμο. |

### Δείτε επίσης

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* χώρος ονομάτων [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* συνέλευση [Aspose.Zip](../../../)


