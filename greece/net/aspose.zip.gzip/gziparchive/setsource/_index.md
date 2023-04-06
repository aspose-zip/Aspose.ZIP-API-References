---
title: GzipArchive.SetSource
second_title: Aspose.ZIP για Αναφορά API .NET
description: GzipArchive μέθοδος. Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου.
type: docs
weight: 70
url: /el/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου.

```csharp
public void SetSource(Stream source)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | Stream | Η ροή εισόδου για το αρχείο. |

### Παραδείγματα

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### Δείτε επίσης

* class [GzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Gzip](../../gziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileInfo | FileInfo | Η αναφορά σε ένα αρχείο που πρόκειται να συμπιεστεί. |

### Παραδείγματα

Ανοίξτε ένα αρχείο από μια ροή και εξαγάγετε το σε ένα`MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### Δείτε επίσης

* class [GzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Gzip](../../gziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου.

```csharp
public void SetSource(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Διαδρομή προς το αρχείο που θα συμπιεστεί. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *path* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*path* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*path* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*path*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*path* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |

### Παραδείγματα

Ανοίξτε ένα αρχείο από αρχείο προς διαδρομή και εξαγάγετε το στο a`MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
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

## SetSource(TarArchive) {#setsource}

Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου.

```csharp
public void SetSource(TarArchive tarArchive)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| tarArchive | TarArchive | Αρχείο πίσσας για συμπίεση. |

### Παρατηρήσεις

Χρησιμοποιήστε αυτήν τη μέθοδο για να δημιουργήσετε κοινό αρχείο tar.gz.

### Παραδείγματα

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var gzippedArchive = new GzipArchive())
    {
           gzippedArchive.SetSource(tarArchive);
           gzippedArchive.Save("archive.tar.gz");
    }
}
```

### Δείτε επίσης

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Gzip](../../gziparchive/)
* συνέλευση [Aspose.Zip](../../../)


