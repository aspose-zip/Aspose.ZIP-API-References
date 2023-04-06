---
title: TarArchive.TarArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: TarArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουTarArchive τάξη.
type: docs
weight: 10
url: /el/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`TarArchive`](../) τάξη.

```csharp
public TarArchive()
```

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει τον τρόπο συμπίεσης ενός αρχείου.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### Δείτε επίσης

* class [TarArchive](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tararchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`Archive`](../../../aspose.zip/archive/) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.

```csharp
public TarArchive(Stream sourceStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. Πρέπει να είναι αναζητήσιμο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| InvalidDataException | *sourceStream* δεν είναι αναζητήσιμο. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυσκευάζει καμία καταχώρηση. Βλέπω[`Open`](../../tarentry/open/)μέθοδος αποσυσκευασίας.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε όλες τις εγγραφές σε έναν κατάλογο.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [TarArchive](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tararchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`TarArchive`](../) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.

```csharp
public TarArchive(string path)
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

Αυτός ο κατασκευαστής δεν αποσυσκευάζει καμία καταχώρηση. Βλέπω[`Open`](../../tarentry/open/)μέθοδος αποσυσκευασίας.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε όλες τις εγγραφές σε έναν κατάλογο.

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [TarArchive](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tararchive/)
* συνέλευση [Aspose.Zip](../../../)


