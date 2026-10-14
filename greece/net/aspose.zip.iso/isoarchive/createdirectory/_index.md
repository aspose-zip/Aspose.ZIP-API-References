---
title: "IsoArchive.CreateDirectory"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος IsoArchive. Προσθέτει έναν φάκελο στην εικόνα ISO"
type: docs
weight: 30
url: /el/net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

Προσθέτει έναν κατάλογο στην εικόνα ISO.

```csharp
public IsoEntry CreateDirectory(string name)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Διαδρομή του φακέλου στο ISO. |

### Τιμή Επιστροφής

Η καταχώρηση ISO δημιουργήθηκε.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Το αρχείο είναι ανοιχτό για εξαγωγή. |
| ArgumentNullException | `name` είναι null ή κενό. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

### Δείτε επίσης

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


