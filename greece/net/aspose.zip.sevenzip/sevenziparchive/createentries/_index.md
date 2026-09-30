---
title: "SevenZipArchive.CreateEntries"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος SevenZipArchive. Προσθέτει στην αρχειοθήκη όλα τα αρχεία και καταλόγους αναδρομικά από τον δοσμένο κατάλογο"
type: docs
weight: 40
url: /el/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοθέντα κατάλογο.

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
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
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| SecurityException | Ο καλούντας δεν διαθέτει την απαιτούμενη άδεια πρόσβασης στο *directory*. |

## Παραδείγματα

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
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοθέντα κατάλογο.

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
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
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentNullException | *sourceDirectory* είναι `null`. |

## Παραδείγματα

Δημιουργήστε μια αρχειοθήκη 7z με συμπίεση LZMA2.

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### Δείτε επίσης

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


