---
title: "XarArchive.CreateEntries"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος XarArchive. Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο"
type: docs
weight: 30
url: /el/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά από τον δοσμένο κατάλογο.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | String | Φάκελος προς συμπίεση. |
| compressionSettings | Boolean | Οι ρυθμίσεις συμπίεσης που χρησιμοποιούνται για τα προστιθέμενα στοιχεία [`XarEntry`](../../xarentry/). |
| includeRootDirectory | XarCompressionSettings | Δείχνει αν θα συμπεριληφθεί ο ριζικός φάκελος ή όχι. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Xar.

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
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### Δείτε επίσης

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά από τον δοσμένο κατάλογο.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | DirectoryInfo | Φάκελος προς συμπίεση. |
| compressionSettings | Boolean | Οι ρυθμίσεις συμπίεσης που χρησιμοποιούνται για τα προστιθέμενα στοιχεία [`XarEntry`](../../xarentry/). |
| includeRootDirectory | XarCompressionSettings | Δείχνει αν θα συμπεριληφθεί ο ριζικός φάκελος ή όχι. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Xar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *directory* είναι null. |
| SecurityException | Ο καλούντας δεν διαθέτει την απαιτούμενη άδεια πρόσβασης στο *directory*. |
| IOException | *directory* αντιπροσωπεύει ένα αρχείο, όχι έναν φάκελο. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### Δείτε επίσης

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


