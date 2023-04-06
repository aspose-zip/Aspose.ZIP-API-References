---
title: SevenZipArchive.CreateEntries
second_title: Aspose.ZIP για Αναφορά API .NET
description: SevenZipArchive μέθοδος. Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.
type: docs
weight: 40
url: /el/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
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
using (SevenZipArchive archive = new SevenZipArchive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.7z");
}
```

### Δείτε επίσης

* class [SevenZipArchive](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον κατάλογο που δίνεται.

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | String | Κατάλογος για συμπίεση. |
| includeRootDirectory | Boolean | Υποδεικνύει εάν θα συμπεριληφθεί ο ίδιος ο ριζικός κατάλογος ή όχι. |

### Επιστρεφόμενη Αξία

Το αρχείο με τις καταχωρήσεις που έχουν συντεθεί.

### Παραδείγματα

Σύνθεση αρχείου 7z με συμπίεση LZMA2.

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### Δείτε επίσης

* class [SevenZipArchive](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)


