---
title: Archive.CreateEntries
second_title: Aspose.ZIP για Αναφορά API .NET
description: Archive μέθοδος. Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.
type: docs
weight: 40
url: /el/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | DirectoryInfo | Κατάλογος για συμπίεση. |
| includeRootDirectory | Boolean | Υποδεικνύει εάν θα συμπεριληφθεί ο ίδιος ο ριζικός κατάλογος ή όχι. |

### Επιστρεφόμενη Αξία

Το αρχείο με τις καταχωρήσεις που έχουν συντεθεί.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| DirectoryNotFoundException | Το μονοπάτι προς*directory* δεν είναι έγκυρο, όπως είναι σε μη αντιστοιχισμένη μονάδα δίσκου. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης*directory*. |

### Παραδείγματα

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
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | String | Κατάλογος για συμπίεση. |
| includeRootDirectory | Boolean | Υποδεικνύει εάν θα συμπεριληφθεί ο ίδιος ο ριζικός κατάλογος ή όχι. |

### Επιστρεφόμενη Αξία

Το αρχείο με τις καταχωρήσεις που έχουν συντεθεί.

### Παραδείγματα

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### Δείτε επίσης

* class [Archive](../)
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)


