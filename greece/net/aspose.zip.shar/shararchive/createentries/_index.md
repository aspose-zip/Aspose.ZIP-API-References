---
title: "SharArchive.CreateEntries"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος SharArchive. Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά από τον δοσμένο φάκελο"
type: docs
weight: 30
url: /el/net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά από τον δοσμένο κατάλογο.

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | String | Φάκελος προς συμπίεση. |
| includeRootDirectory | Boolean | Δείχνει αν θα συμπεριληφθεί ο ριζικός φάκελος ή όχι. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Shar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *sourceDirectory* είναι null. |
| SecurityException | Ο καλούν δεν διαθέτει την απαιτούμενη άδεια για πρόσβαση στο *sourceDirectory*. |
| ArgumentException | *sourceDirectory* περιέχει μη έγκυρους χαρακτήρες όπως ", &lt;, &gt;, ή &#x7C;. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι μικρότερα από 260 χαρακτήρες. Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο είναι πολύ μεγάλα. |
| IOException | *sourceDirectory* αντιπροσωπεύει ένα αρχείο, όχι έναν φάκελο. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(sharFile);
    }
}
```

### Δείτε επίσης

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά από τον δοσμένο κατάλογο.

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | DirectoryInfo | Φάκελος προς συμπίεση. |
| includeRootDirectory | Boolean | Δείχνει αν θα συμπεριληφθεί ο ριζικός φάκελος ή όχι. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Shar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *directory* είναι null. |
| SecurityException | Ο καλούντας δεν διαθέτει την απαιτούμενη άδεια πρόσβασης στο *directory*. |
| IOException | *directory* αντιπροσωπεύει ένα αρχείο, όχι έναν φάκελο. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(sharFile);
    }
}
```

### Δείτε επίσης

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


