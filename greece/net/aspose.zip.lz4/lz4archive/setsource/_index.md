---
title: "Lz4Archive.SetSource"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Lz4Archive μέθοδος. Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο"
type: docs
weight: 70
url: /el/net/aspose.zip.lz4/lz4archive/setsource/
---
## SetSource(Stream) {#setsource_2}

Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```csharp
public void SetSource(Stream source)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | Stream | Η ροή εισόδου για το αρχείο. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για εξαγωγή. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

```csharp
using (var archive = new Lz4Archive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz4");
}
```

### Δείτε επίσης

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileInfo | FileInfo | Η αναφορά σε ένα αρχείο που θα συμπιεστεί. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για εξαγωγή. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

Ανοίξτε ένα αρχείο από μια ροή και εξάγετέ το σε ένα `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz4");
}
```

### Δείτε επίσης

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource}

Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| tarArchive | TarArchive | Αρχείο Tar προς συμπίεση. |
| μορφή | TarFormat | Ορίζει τη μορφή της κεφαλίδας tar. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Αυτό το αρχείο είναι προετοιμασμένο για εξαγωγή. |

## Παρατηρήσεις

Χρησιμοποιήστε αυτή τη μέθοδο για να συνθέσετε κοινό αρχείο tar.lz4.

## Παραδείγματα

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var lz4Archive = new Lz4Archive())
    {
        lz4Archive.SetSource(tarArchive);
        lz4Archive.Save("archive.tar.lz4");
    }
}
```

### Δείτε επίσης

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```csharp
public void SetSource(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Διαδρομή προς το αρχείο που θα συμπιεστεί. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| SecurityException | Ο καλών δεν διαθέτει τα απαιτούμενα δικαιώματα πρόσβασης. |
| ArgumentException | Η *path* είναι κενή, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Η πρόσβαση στο αρχείο *path* απορρίπτεται. |
| PathTooLongException | Η καθορισμένη *path*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| NotSupportedException | Το αρχείο στο *path* περιέχει άνω τελεία (:) στη μέση της συμβολοσειράς. |
| InvalidOperationException | Αυτό το αρχείο είναι προετοιμασμένο για εξαγωγή. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

Ανοίξτε ένα αρχείο από διαδρομή και εξάγετε το σε ένα `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Δείτε επίσης

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


