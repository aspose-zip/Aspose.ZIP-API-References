---
title: "TarArchive.FromZstandard"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος TarArchive. Εξάγει το παρεχόμενο αρχείο Zstandard και συνθέτει TarArchive από τα εξαγόμενα δεδομένα."
type: docs
weight: 80
url: /el/net/aspose.zip.tar/tararchive/fromzstandard/
---
## FromZstandard(Stream) {#fromzstandard}

Εξάγει το παρεχόμενο αρχείο Zstandard και συνθέτει [`TarArchive`](../) από τα εξαγόμενα δεδομένα.

Σημαντικό: Το αρχείο Zstandard εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

```csharp
public static TarArchive FromZstandard(Stream source)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | Stream | Η πηγή του αρχείου. |

### Τιμή Επιστροφής

Μια παρουσία του [`TarArchive`](../)

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| IOException | Η ροή Zstandard είναι κατεστραμμένη ή μη αναγνώσιμη. |
| InvalidDataException | Τα δεδομένα είναι κατεστραμμένα. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |

### Δείτε επίσης

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZstandard(string) {#fromzstandard_1}

Εξάγει το παρεχόμενο αρχείο Zstandard και συνθέτει [`TarArchive`](../) από τα εξαγόμενα δεδομένα.

Σημαντικό: Το αρχείο Zstandard εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

```csharp
public static TarArchive FromZstandard(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η διαδρομή προς το αρχείο αρχειοθήκης. |

### Τιμή Επιστροφής

Μια παρουσία του [`TarArchive`](../)

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* βρίσκεται σε μη έγκυρη μορφή. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| IOException | Η ροή Zstandard είναι κατεστραμμένη ή μη αναγνώσιμη. |
| InvalidDataException | Τα δεδομένα είναι κατεστραμμένα. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |

### Δείτε επίσης

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


