---
title: "IsoArchive.ExtractToDirectory"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος IsoArchive. Εξάγει όλες τις καταχωρήσεις στον καθορισμένο φάκελο"
type: docs
weight: 60
url: /el/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

Εξάγει όλες τις καταχωρήσεις στον καθορισμένο κατάλογο.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | String | Ο φάκελος στον οποίο θα εξαχθούν οι καταχωρήσεις. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εκτοπίζεται όταν το αρχείο είναι σε λειτουργία επεξεργασίας. |
| ArgumentNullException | Εκτοπίζεται όταν η *destinationDirectory* είναι null. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


