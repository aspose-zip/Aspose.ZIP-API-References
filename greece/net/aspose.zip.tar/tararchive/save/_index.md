---
title: "TarArchive.Save"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος TarArchive. Αποθηκεύει το αρχείο στη δοθείσα ροή"
type: docs
weight: 150
url: /el/net/aspose.zip.tar/tararchive/save/
---
## Save(Stream, TarFormat?) {#save}

Αποθηκεύει την αρχειοθήκη στη δοθείσα ροή.

```csharp
public void Save(Stream output, TarFormat? format = default)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |
| μορφή | Nullable`1 | Ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | *output* δεν είναι εγγράψιμο. - ή - *output* είναι η ίδια ροή από την οποία εξάγουμε. Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί - Ή - Είναι αδύνατο να αποθηκευτεί το αρχείο σε *format* λόγω περιορισμών μορφής. |

## Παρατηρήσεις

*output* must be writable.

## Παραδείγματα

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry1", "data.bin");
        archive.Save(tarFile);
    }
}       
```

### Δείτε επίσης

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, TarFormat?) {#save_1}

Αποθηκεύει το αρχείο σε προορισμένο αρχείο που παρέχεται.

```csharp
public void Save(string destinationFileName, TarFormat? format = default)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| μορφή | Nullable`1 | Ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν. |

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
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί και δεν μπορεί να χρησιμοποιηθεί |

## Παρατηρήσεις

Είναι δυνατόν να αποθηκεύσετε ένα αρχείο στην ίδια διαδρομή από την οποία φορτώθηκε. Ωστόσο, αυτό δεν συνιστάται επειδή αυτή η προσέγγιση χρησιμοποιεί αντιγραφή σε προσωρινό αρχείο.

## Παραδείγματα

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("myarchive.tar");
}       
```

### Δείτε επίσης

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


