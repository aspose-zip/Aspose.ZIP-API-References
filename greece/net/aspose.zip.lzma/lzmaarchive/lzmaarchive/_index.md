---
title: LzmaArchive.LzmaArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: LzmaArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουLzmaArchive τάξη και συνθέτει το αρχείο σε μορφή lzma.
type: docs
weight: 10
url: /el/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`LzmaArchive`](../) τάξη και συνθέτει το αρχείο σε μορφή lzma.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| settings | LzmaArchiveSettings | Σύνολο ρύθμισης συγκεκριμένου αρχείου lzma. |

### Δείτε επίσης

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* χώρος ονομάτων [Aspose.Zip.LZMA](../../lzmaarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`LzmaArchive`](../) τάξη προετοιμασμένη για αποσυμπίεση.

```csharp
public LzmaArchive(Stream source)
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

* class [LzmaArchive](../)
* χώρος ονομάτων [Aspose.Zip.LZMA](../../lzmaarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`LzmaArchive`](../) τάξη προετοιμασμένη για αποσυμπίεση.

```csharp
public LzmaArchive(string path)
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

### Παραδείγματα

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Δείτε επίσης

* class [LzmaArchive](../)
* χώρος ονομάτων [Aspose.Zip.LZMA](../../lzmaarchive/)
* συνέλευση [Aspose.Zip](../../../)


