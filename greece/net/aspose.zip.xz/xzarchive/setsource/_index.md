---
title: XzArchive.SetSource
second_title: Aspose.ZIP για Αναφορά API .NET
description: XzArchive μέθοδος. Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου.
type: docs
weight: 50
url: /el/net/aspose.zip.xz/xzarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου.

```csharp
public void SetSource(Stream source)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | Stream | Η ροή εισόδου για το αρχείο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | ο*source* το ρεύμα είναι αζήτητο. |

### Παραδείγματα

```csharp
using (var archive = new XzArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.xz");
}
```

### Δείτε επίσης

* class [XzArchive](../)
* χώρος ονομάτων [Aspose.Zip.Xz](../../xzarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo που θα ανοίξει ως ροή εισόδου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια για να ανοίξει το*fileInfo*. |
| ArgumentException | Η διαδρομή αρχείου είναι κενή ή περιέχει μόνο λευκά κενά. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| UnauthorizedAccessException | Η διαδρομή προς το αρχείο είναι μόνο για ανάγνωση ή είναι κατάλογος. |
| ArgumentNullException | *fileInfo* είναι μηδενικό. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή δεν είναι έγκυρη, όπως είναι σε μη αντιστοιχισμένη μονάδα δίσκου. |
| IOException | Το αρχείο είναι ήδη ανοιχτό. |

### Παραδείγματα

```csharp
using (var archive = new XzArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.xz");
}
```

### Δείτε επίσης

* class [XzArchive](../)
* χώρος ονομάτων [Aspose.Zip.Xz](../../xzarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Ορίζει το περιεχόμενο που θα συμπιέζεται εντός του αρχείου.

```csharp
public void SetSource(string sourcePath)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourcePath | String | Διαδρομή προς το αρχείο που θα ανοίξει ως ροή εισόδου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *sourcePath* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*sourcePath* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*sourcePath* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*sourcePath*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*sourcePath* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |

### Παραδείγματα

```csharp
using (var archive = new XzArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.xz");
}
```

### Δείτε επίσης

* class [XzArchive](../)
* χώρος ονομάτων [Aspose.Zip.Xz](../../xzarchive/)
* συνέλευση [Aspose.Zip](../../../)


