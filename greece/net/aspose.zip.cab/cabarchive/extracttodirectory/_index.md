---
title: "CabArchive.ExtractToDirectory"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "CabArchive μέθοδος. Εξάγει όλα τα αρχεία στο αρχείο στον παρεχόμενο κατάλογο."
type: docs
weight: 60
url: /el/net/aspose.zip.cab/cabarchive/extracttodirectory/
---
## CabArchive.ExtractToDirectory method

Εξάγει όλα τα αρχεία στην αρχειοθήκη στον παρεχόμενο κατάλογο.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | String | Η διαδρομή προς το φάκελο όπου θα τοποθετηθούν τα εξαγόμενα αρχεία. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | η διαδρομή είναι null |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. |
| SecurityException | Ο καλών δεν διαθέτει τα απαιτούμενα δικαιώματα για πρόσβαση στον υπάρχον φάκελο. |
| NotSupportedException | Εάν ο φάκελος δεν υπάρχει, μια διαδρομή περιέχει χαρακτήρα άνω-κάτω τελείας (:) που δεν αποτελεί μέρος ετικέτας μονάδας (\"C:\\\\"). |
| ArgumentException | Η διαδρομή είναι κενή συμβολοσειρά, περιέχει μόνο κενά διαστήματα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες. Μπορείτε να ελέγξετε για μη έγκυρους χαρακτήρες χρησιμοποιώντας τη μέθοδο System.IO.Path.GetInvalidPathChars. -ή- η διαδρομή αρχίζει ή περιέχει μόνο χαρακτήρα άνω-κάτω τελείας (:). |
| IOException | Ο φάκελος που καθορίζεται από τη διαδρομή είναι αρχείο. -or- Το όνομα δικτύου είναι άγνωστο. |
| InvalidDataException | Το αρχείο είναι κατεστραμμένο. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για σύνθεση και δεν μπορεί να εξαχθεί. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |

## Παρατηρήσεις

Εάν ο φάκελος δεν υπάρχει, θα δημιουργηθεί.

## Παραδείγματα

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


