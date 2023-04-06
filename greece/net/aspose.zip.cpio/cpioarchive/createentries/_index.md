---
title: CpioArchive.CreateEntries
second_title: Aspose.ZIP για Αναφορά API .NET
description: CpioArchive μέθοδος. Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.
type: docs
weight: 30
url: /el/net/aspose.zip.cpio/cpioarchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.

```csharp
public CpioArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | String | Κατάλογος για συμπίεση. |
| includeRootDirectory | Boolean | Υποδεικνύει εάν θα συμπεριληφθεί ο ίδιος ο ριζικός κατάλογος ή όχι. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής Cpio.

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
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(cpioFile);
    }
}
```

### Δείτε επίσης

* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.

```csharp
public CpioArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | DirectoryInfo | Κατάλογος για συμπίεση. |
| includeRootDirectory | Boolean | Υποδεικνύει εάν θα συμπεριληφθεί ο ίδιος ο ριζικός κατάλογος ή όχι. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής Cpio.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *directory* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης*directory*. |
| IOException | *directory* σημαίνει αρχείο, όχι κατάλογο. |

### Παραδείγματα

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(cpioFile);
    }
}
```

### Δείτε επίσης

* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)


