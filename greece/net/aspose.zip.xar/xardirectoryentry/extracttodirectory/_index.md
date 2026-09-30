---
title: "XarDirectoryEntry.ExtractToDirectory"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος XarDirectoryEntry. Εξάγει όλα τα αρχεία στον τρέχοντα κατάλογο στον παρεχόμενο κατάλογο"
type: docs
weight: 50
url: /el/net/aspose.zip.xar/xardirectoryentry/extracttodirectory/
---
## XarDirectoryEntry.ExtractToDirectory method

Αποσυμπιέζει όλα τα αρχεία στον τρέχοντα κατάλογο στον παρεχόμενο κατάλογο.

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
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| SecurityException | Ο καλών δεν διαθέτει τα απαιτούμενα δικαιώματα για πρόσβαση στον υπάρχον φάκελο. |
| NotSupportedException | Εάν ο φάκελος δεν υπάρχει, η διαδρομή περιέχει χαρακτήρα άνω-κάθετο (:) που δεν αποτελεί μέρος ετικέτας μονάδας (\"C:\\"). |
| ArgumentException | Η διαδρομή είναι κενή συμβολοσειρά, περιέχει μόνο κενά διαστήματα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες. Μπορείτε να ελέγξετε για μη έγκυρους χαρακτήρες χρησιμοποιώντας τη μέθοδο System.IO.Path.GetInvalidPathChars. -ή- η διαδρομή αρχίζει ή περιέχει μόνο χαρακτήρα άνω-κάτω τελείας (:). |
| IOException | Ο φάκελος που καθορίζεται από τη διαδρομή είναι αρχείο. -or- Το όνομα δικτύου είναι άγνωστο. |
| InvalidDataException | Το αρχείο είναι κατεστραμμένο. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |

## Παρατηρήσεις

Εάν ο φάκελος δεν υπάρχει, θα δημιουργηθεί.

## Παραδείγματα

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   ((XarDirectoryEntry)archive.Entries[0]).ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [XarDirectoryEntry](../)
* namespace [Aspose.Zip.Xar](../../xardirectoryentry/)
* assembly [Aspose.Zip](../../../)


