---
title: "ArjArchive.ExtractToDirectory"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος ArjArchive. Εξάγει όλες τις καταχωρήσεις στον καθορισμένο φάκελο"
type: docs
weight: 60
url: /el/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

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
| ArgumentNullException | Εκτοπίζεται όταν η *destinationDirectory* είναι null. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |
| InvalidDataException | Ασυμφωνία αθροίσματος ελέγχου για κεφαλίδες ή δεδομένα. - ή - Το αρχείο είναι κατεστραμμένο. |
| NotImplementedException | Καταχώρηση συμπιεσμένη με μέθοδο 4. |

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις καταχωρήσεις σε έναν φάκελο:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


