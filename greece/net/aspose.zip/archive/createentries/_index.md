---
title: "Archive.CreateEntries"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος Archive. Προσθέτει στο αρχείο όλα τα αρχεία και τους φακέλους αναδρομικά στον δοσμένο φάκελο."
type: docs
weight: 50
url: /el/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Προσθέτει στην αρχειοθήκη όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | DirectoryInfo | Φάκελος προς συμπίεση. |
| includeRootDirectory | Boolean | Δείχνει αν θα συμπεριληφθεί ο ριζικός φάκελος ή όχι. |

### Τιμή Επιστροφής

Το αρχείο με τις συντεθειμένες καταχωρήσεις.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| DirectoryNotFoundException | Η διαδρομή προς *directory* είναι άκυρη, όπως όταν βρίσκεται σε μη συνδεδεμένο δίσκο. |
| SecurityException | Ο καλούντας δεν διαθέτει την απαιτούμενη άδεια πρόσβασης στο *directory*. |
| ObjectDisposedException | Εκτοπίζεται εάν το αρχείο έχει διαγραφεί. |
| ArgumentNullException | *directory* είναι `null`. |

## Παραδείγματα

```csharp
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### Δείτε επίσης

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Προσθέτει στην αρχειοθήκη όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | String | Φάκελος προς συμπίεση. |
| includeRootDirectory | Boolean | Δείχνει αν θα συμπεριληφθεί ο ριζικός φάκελος ή όχι. |

### Τιμή Επιστροφής

Το αρχείο με τις συντεθειμένες καταχωρήσεις.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Εκτοπίζεται εάν το αρχείο έχει διαγραφεί. |
| ArgumentException | *sourceDirectory* περιέχει μη έγκυρους χαρακτήρες όπως ", &lt;, &gt;, ή &#x7C;. |
| ArgumentNullException | *sourceDirectory* είναι `null`. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. |

## Παραδείγματα

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### Δείτε επίσης

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


