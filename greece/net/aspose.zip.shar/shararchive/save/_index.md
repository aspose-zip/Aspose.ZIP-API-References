---
title: "SharArchive.Save"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "SharArchive method. Αποθηκεύει το αρχείο σε ένα αρχείο προορισμού που παρέχεται"
type: docs
weight: 70
url: /el/net/aspose.zip.shar/shararchive/save/
---
## Save(string) {#save_1}

Αποθηκεύει το αρχείο σε προορισμένο αρχείο που παρέχεται.

```csharp
public void Save(string destinationFileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *destinationFileName* είναι μια συμβολοσειρά μηδενικού μήκους, περιέχει μόνο κενά διαστήματα ή περιέχει έναν ή περισσότερους μη έγκυρους χαρακτήρες όπως ορίζονται από System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* είναι null. |
| PathTooLongException | Το καθορισμένο *destinationFileName*, το όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που ορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες βασισμένες στα Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων μικρότερα από 260 χαρακτήρες. |
| DirectoryNotFoundException | Το καθορισμένο *destinationFileName* δεν είναι έγκυρο, (π.χ., βρίσκεται σε μη αντιστοιχισμένο δίσκο). |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά το άνοιγμα του αρχείου. |
| UnauthorizedAccessException | *destinationFileName* καθόρισε ένα αρχείο μόνο για ανάγνωση και η πρόσβαση δεν είναι Read.-ή- η διαδρομή καθόρισε έναν φάκελο.-ή- ο καλών δεν διαθέτει την απαιτούμενη άδεια. |
| NotSupportedException | *destinationFileName* βρίσκεται σε μη έγκυρη μορφή. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Αυτό το αρχείο είναι ανοιχτό για εξαγωγή. |

## Παρατηρήσεις

Είναι δυνατόν να αποθηκεύσετε ένα αρχείο στην ίδια διαδρομή από την οποία φορτώθηκε. Ωστόσο, αυτό δεν συνιστάται επειδή αυτή η προσέγγιση χρησιμοποιεί αντιγραφή σε προσωρινό αρχείο.

## Παραδείγματα

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### Δείτε επίσης

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή.

```csharp
public void Save(Stream output)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *output* είναι null. |
| ArgumentException | *output* δεν είναι εγγράψιμο. - ή - *output* είναι η ίδια ροή από την οποία εξάγουμε. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Αυτό το αρχείο είναι ανοιχτό για εξαγωγή. |

## Παρατηρήσεις

*output* must be writable.

## Παραδείγματα

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### Δείτε επίσης

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


