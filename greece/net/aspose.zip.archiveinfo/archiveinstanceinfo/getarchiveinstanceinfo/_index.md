---
title: ArchiveInstanceInfo.GetArchiveInstanceInfo
second_title: Aspose.ZIP για Αναφορά API .NET
description: ArchiveInstanceInfo μέθοδος. Λαμβάνει πληροφορίες παρουσίας αρχείου.
type: docs
weight: 10
url: /el/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

Λαμβάνει πληροφορίες παρουσίας αρχείου.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Το όνομα αρχείου του αρχείου αρχειοθέτησης. |

### Επιστρεφόμενη Αξία

Πληροφορίες σχετικά με την παρουσία αρχειοθέτησης ή μηδενική εάν δεν εντοπίστηκε μορφή.

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

* class [ArchiveInstanceInfo](../)
* χώρος ονομάτων [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* συνέλευση [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

Λαμβάνει πληροφορίες παρουσίας αρχείου.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή του αρχείου αρχείου. |

### Επιστρεφόμενη Αξία

Πληροφορίες σχετικά με την παρουσία αρχειοθέτησης ή μηδενική εάν δεν εντοπίστηκε μορφή.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *stream* είναι μηδενικό. |
| ArgumentException | *stream* δεν είναι αναζητήσιμο. |

### Δείτε επίσης

* class [ArchiveInstanceInfo](../)
* χώρος ονομάτων [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* συνέλευση [Aspose.Zip](../../../)


