---
title: CpioArchive.CpioArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: CpioArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουCpioArchive τάξη.
type: docs
weight: 10
url: /el/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`CpioArchive`](../) τάξη.

```csharp
public CpioArchive()
```

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει τον τρόπο συμπίεσης ενός αρχείου.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Δείτε επίσης

* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`CpioArchive`](../) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.

```csharp
public CpioArchive(Stream sourceStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. Πρέπει να είναι αναζητήσιμο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *sourceStream* είναι μηδενικό. |
| ArgumentException | *sourceStream* δεν είναι αναζητήσιμο. |
| InvalidDataException | *sourceStream* δεν είναι έγκυρο αρχείο cpio. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυσκευάζει καμία καταχώρηση. Βλέπω[`Open`](../../cpioentry/open/)μέθοδος αποσυσκευασίας.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε όλες τις εγγραφές σε έναν κατάλογο.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`CpioArchive`](../) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.

```csharp
public CpioArchive(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η διαδρομή προς το αρχείο αρχειοθέτησης. |

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

Αυτός ο κατασκευαστής δεν αποσυσκευάζει καμία καταχώρηση. Βλέπω[`Open`](../../cpioentry/open/)μέθοδος αποσυσκευασίας.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε όλες τις εγγραφές σε έναν κατάλογο.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)


