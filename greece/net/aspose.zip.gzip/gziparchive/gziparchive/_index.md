---
title: GzipArchive.GzipArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: GzipArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουGzipArchive τάξη προετοιμασμένη για συμπίεση.
type: docs
weight: 10
url: /el/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`GzipArchive`](../) τάξη προετοιμασμένη για συμπίεση.

```csharp
public GzipArchive()
```

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Δείτε επίσης

* class [GzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Gzip](../../gziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`GzipArchive`](../) τάξη προετοιμασμένη για αποσυμπίεση.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| parseHeader | Boolean | Εάν θα αναλυθεί η κεφαλίδα ροής για να καταλάβουμε ιδιότητες, συμπεριλαμβανομένου του ονόματος. Είναι λογικό μόνο για ροή με δυνατότητα αναζήτησης. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζεται. Βλέπω[`Open`](../open/) μέθοδος αποσυμπίεσης.

### Παραδείγματα

Ανοίξτε ένα αρχείο από μια ροή και εξαγάγετε το σε ένα`MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### Δείτε επίσης

* class [GzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Gzip](../../gziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`GzipArchive`](../) τάξη.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η διαδρομή προς το αρχείο αρχειοθέτησης. |
| parseHeader | Boolean | Εάν θα αναλυθεί η κεφαλίδα ροής για να καταλάβουμε ιδιότητες, συμπεριλαμβανομένου του ονόματος. Είναι λογικό μόνο για ροή με δυνατότητα αναζήτησης. |

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

Αυτός ο κατασκευαστής δεν αποσυμπιέζεται. Βλέπω[`Open`](../open/) μέθοδος αποσυμπίεσης.

### Παραδείγματα

Ανοίξτε ένα αρχείο από αρχείο προς διαδρομή και εξαγάγετε το στο a`MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### Δείτε επίσης

* class [GzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Gzip](../../gziparchive/)
* συνέλευση [Aspose.Zip](../../../)


