---
title: LzipArchive.LzipArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: LzipArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουLzipArchive .
type: docs
weight: 10
url: /el/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`LzipArchive`](../) .

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| settings | LzipArchiveSettings | Ρύθμιση συγκεκριμένου αρχείου lzip με ορισμό μεγέθους λεξικού. |

### Δείτε επίσης

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Lzip](../../lziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## LzipArchive(Stream) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`LzipArchive`](../) τάξη προετοιμασμένη για αποσυμπίεση.

```csharp
public LzipArchive(Stream sourceStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *sourceStream* δεν είναι αναζητήσιμο. |
| ArgumentNullException | *sourceStream* είναι μηδενικό. |
| InvalidDataException | Οι κεφαλίδες δεν ταιριάζουν με τον τύπο αρχείου lzip. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζεται. Βλέπω[`Extract`](../extract/) μέθοδος αποσυμπίεσης.

### Δείτε επίσης

* class [LzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Lzip](../../lziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## LzipArchive(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`LzipArchive`](../) τάξη προετοιμασμένη για αποσυμπίεση.

```csharp
public LzipArchive(string path)
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
| InvalidDataException | Οι κεφαλίδες δεν ταιριάζουν με τον τύπο αρχείου lzip. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζεται. Βλέπω[`Extract`](../extract/) μέθοδος αποσυμπίεσης.

### Παραδείγματα

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### Δείτε επίσης

* class [LzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Lzip](../../lziparchive/)
* συνέλευση [Aspose.Zip](../../../)


