---
title: "XarArchive.DeleteEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος XarArchive. Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων."
type: docs
weight: 50
url: /el/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| καταχώρηση | XarEntry | Η καταχώρηση που θα αφαιρεθεί από τη λίστα καταχωρήσεων. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Xar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *entry* είναι null. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Το αρχείο δεν είναι ανοιχτό για εξαγωγή. |

## Παραδείγματα

Ακολουθεί ο τρόπος για να αφαιρέσετε όλες τις καταχωρήσεις εκτός από την τελευταία:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### Δείτε επίσης

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


