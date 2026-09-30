---
title: "SevenZipArchive.ExtractToDirectory"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "SevenZipArchive μέθοδος. Εξάγει όλα τα αρχεία στο αρχείο στον παρεχόμενο κατάλογο."
type: docs
weight: 70
url: /el/net/aspose.zip.sevenzip/sevenziparchive/extracttodirectory/
---
## SevenZipArchive.ExtractToDirectory method

Εξάγει όλα τα αρχεία στην αρχειοθήκη στον παρεχόμενο κατάλογο.

```csharp
public void ExtractToDirectory(string destinationDirectory, string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | String | Η διαδρομή προς το φάκελο όπου θα τοποθετηθούν τα εξαγόμενα αρχεία. |
| password | String | Προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση περιεχομένου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *destinationDirectory* είναι null. |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| SecurityException | Ο καλών δεν διαθέτει τα απαιτούμενα δικαιώματα για πρόσβαση στον υπάρχον φάκελο. |
| NotSupportedException | Εάν ο φάκελος δεν υπάρχει, η διαδρομή περιέχει χαρακτήρα άνω-κάθετο (:) που δεν αποτελεί μέρος ετικέτας μονάδας (\"C:\\"). |
| ArgumentException | *destinationDirectory* είναι συμβολοσειρά μηδενικού μήκους, περιέχει μόνο κενά διαστήματα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες. Μπορείτε να ερωτήσετε για μη έγκυρους χαρακτήρες χρησιμοποιώντας τη μέθοδο System.IO.Path.GetInvalidPathChars. -or- η διαδρομή προέρχεται ή περιέχει μόνο χαρακτήρα άνω-κάθετο (:). |
| IOException | Ο φάκελος που καθορίζεται από τη διαδρομή είναι αρχείο. -or- Το όνομα δικτύου είναι άγνωστο. |
| InvalidDataException | Το αρχείο είναι κατεστραμμένο. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |

## Παρατηρήσεις

Εάν ο φάκελος δεν υπάρχει, θα δημιουργηθεί.

*password* is used for content decryption only. If file names are encrypted provide password in [`SevenZipArchive`](../sevenziparchive/), [`SevenZipArchive`](../sevenziparchive/), [`SevenZipArchive`](../sevenziparchive/) or [`SevenZipArchive`](../sevenziparchive/) constructor.

## Παραδείγματα

```csharp
using (var archive = new SevenZipArchive("archive.7z")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Δείτε επίσης

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


