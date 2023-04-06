---
title: SharArchive.CreateEntries
second_title: Aspose.ZIP για Αναφορά API .NET
description: SharArchive μέθοδος. Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.
type: docs
weight: 30
url: /el/net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | String | Κατάλογος για συμπίεση. |
| includeRootDirectory | Boolean | Υποδεικνύει εάν θα συμπεριληφθεί ο ίδιος ο ριζικός κατάλογος ή όχι. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής Shar.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *sourceDirectory* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης*sourceDirectory*. |
| ArgumentException | *sourceDirectory* περιέχει μη έγκυρους χαρακτήρες όπως ", &lt;, &gt; ή &#x7C;. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο είναι πολύ μεγάλα. |
| IOException | *sourceDirectory* σημαίνει αρχείο, όχι κατάλογο. |

### Παραδείγματα

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
* χώρος ονομάτων [Aspose.Zip.Shar](../../shararchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | DirectoryInfo | Κατάλογος για συμπίεση. |
| includeRootDirectory | Boolean | Υποδεικνύει εάν θα συμπεριληφθεί ο ίδιος ο ριζικός κατάλογος ή όχι. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής Shar.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *directory* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης*directory*. |
| IOException | *directory* σημαίνει αρχείο, όχι κατάλογο. |

### Παραδείγματα

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
* χώρος ονομάτων [Aspose.Zip.Shar](../../shararchive/)
* συνέλευση [Aspose.Zip](../../../)


