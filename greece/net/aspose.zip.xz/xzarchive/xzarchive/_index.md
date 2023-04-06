---
title: XzArchive.XzArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: XzArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουXzArchive τάξη και συνθέτει το αρχείο σε μορφή xz.
type: docs
weight: 10
url: /el/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`XzArchive`](../) τάξη και συνθέτει το αρχείο σε μορφή xz.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| settings | XzArchiveSettings | Σύνολο ρύθμισης συγκεκριμένου αρχείου xz: μέγεθος λεξικού, μέγεθος μπλοκ, τύπος ελέγχου. |

### Δείτε επίσης

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* χώρος ονομάτων [Aspose.Zip.Xz](../../xzarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`XzArchive`](../) τάξη προετοιμασμένη για αποσυμπίεση.

```csharp
public XzArchive(Stream source)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | Stream | Η πηγή του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *source* δεν είναι αναζητήσιμο. |
| ArgumentNullException | *source* είναι μηδενικό. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζεται. Βλέπω[`Extract`](../extract/) μέθοδος αποσυμπίεσης.

### Δείτε επίσης

* class [XzArchive](../)
* χώρος ονομάτων [Aspose.Zip.Xz](../../xzarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`XzArchive`](../) τάξη προετοιμασμένη για αποσυμπίεση.

```csharp
public XzArchive(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Διαδρομή προς την πηγή του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *path* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*path* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*path* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*path*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*path* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζεται. Βλέπω[`Extract`](../extract/) μέθοδος αποσυμπίεσης.

### Δείτε επίσης

* class [XzArchive](../)
* χώρος ονομάτων [Aspose.Zip.Xz](../../xzarchive/)
* συνέλευση [Aspose.Zip](../../../)


