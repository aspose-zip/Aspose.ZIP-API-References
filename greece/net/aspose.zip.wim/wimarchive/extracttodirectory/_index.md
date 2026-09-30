---
title: "WimArchive.ExtractToDirectory"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "WimArchive μέθοδος. Εξάγει το αρχείο στην τοποθεσία που καθορίζεται από τη διαδρομή"
type: docs
weight: 90
url: /el/net/aspose.zip.wim/wimarchive/extracttodirectory/
---
## WimArchive.ExtractToDirectory method

Εξάγει το αρχείο στο αρχείο με βάση τη διαδρομή.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | String | Η διαδρομή προς το φάκελο όπου θα τοποθετηθούν τα εξαγόμενα αρχεία. |

### Τιμή Επιστροφής

Πληροφορίες του εξαγόμενου αρχείου.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentNullException | *destinationDirectory* είναι null |
| PathTooLongException | Η καθορισμένη διαδρομή, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| SecurityException | Ο καλών δεν διαθέτει τα απαιτούμενα δικαιώματα για πρόσβαση στον υπάρχον φάκελο. |
| NotSupportedException | Εάν ο φάκελος δεν υπάρχει, η διαδρομή περιέχει χαρακτήρα άνω-κάτω τελείας (:) που δεν αποτελεί μέρος ετικέτας μονάδας ("C:\") - ή - το αρχείο WIM είναι πολυτμηματικό. |
| ArgumentException | Η διαδρομή είναι κενή συμβολοσειρά, περιέχει μόνο κενά διαστήματα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες. Μπορείτε να ελέγξετε για μη έγκυρους χαρακτήρες χρησιμοποιώντας τη μέθοδο System.IO.Path.GetInvalidPathChars. -ή- η διαδρομή αρχίζει ή περιέχει μόνο χαρακτήρα άνω-κάτω τελείας (:). |
| IOException | Ο φάκελος που καθορίζεται από τη διαδρομή είναι αρχείο. -or- Το όνομα δικτύου είναι άγνωστο. |
| InvalidDataException | Το αρχείο είναι κατεστραμμένο. |
| OperationCanceledException | Στο .NET Framework 4.0 και άνω: Εκτοπίζεται όταν η εξαγωγή ακυρώνεται μέσω του παρεχόμενου διακριτικού ακύρωσης. |

### Δείτε επίσης

* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)


