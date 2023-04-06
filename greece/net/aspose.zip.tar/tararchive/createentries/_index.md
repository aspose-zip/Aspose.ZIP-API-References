---
title: TarArchive.CreateEntries
second_title: Aspose.ZIP για Αναφορά API .NET
description: TarArchive μέθοδος. Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.
type: docs
weight: 70
url: /el/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | DirectoryInfo | Κατάλογος για συμπίεση. |
| includeRootDirectory | Boolean | Υποδεικνύει εάν θα συμπεριληφθεί ο ίδιος ο ριζικός κατάλογος ή όχι. |

### Επιστρεφόμενη Αξία

Το αρχείο με τις καταχωρήσεις που έχουν συντεθεί.

### Παραδείγματα

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### Δείτε επίσης

* class [TarArchive](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tararchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | String | Κατάλογος για συμπίεση. |
| includeRootDirectory | Boolean | Υποδεικνύει εάν θα συμπεριληφθεί ο ίδιος ο ριζικός κατάλογος ή όχι. |

### Επιστρεφόμενη Αξία

Το αρχείο με τις καταχωρήσεις που έχουν συντεθεί.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *sourceDirectory* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης*sourceDirectory*. |
| ArgumentException | *sourceDirectory* περιέχει μη έγκυρους χαρακτήρες όπως ", &lt;, &gt; ή &#x7C;. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο είναι πολύ μεγάλα. |

### Παραδείγματα

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### Δείτε επίσης

* class [TarArchive](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tararchive/)
* συνέλευση [Aspose.Zip](../../../)


