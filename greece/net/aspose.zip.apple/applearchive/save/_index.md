---
title: "AppleArchive.Save"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "AppleArchive μέθοδος. Αποθηκεύει το αρχείο στη δοθείσα ροή"
type: docs
weight: 90
url: /el/net/aspose.zip.apple/applearchive/save/
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
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί. |
| ArgumentNullException | *output* είναι `null`. |
| ArgumentException | *output* δεν είναι εγγράψιμο. |
| ArgumentOutOfRangeException | Το διαμορφωμένο μέγεθος μπλοκ LZ4 ή Zlib δεν είναι θετικό. |
| NotSupportedException | Οι ρυθμίσεις συμπίεσης λείπουν ή δεν υποστηρίζονται, η άμεση σύνθεση χρησιμοποιεί μια ροή που δεν υποστηρίζει αναζήτηση, ή το μέγεθος της καταχώρισης/αρχείου υπερβαίνει τα τρέχοντα όρια του Apple Archive. |

## Παρατηρήσεις

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### Δείτε επίσης

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Αποθηκεύει το αρχείο σε προορισμένο αρχείο που παρέχεται.

```csharp
public void Save(string destinationFileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί. |
| ArgumentException | *destinationFileName* είναι άκυρο. |
| ArgumentNullException | *destinationFileName* είναι `null`. |
| ArgumentOutOfRangeException | Το διαμορφωμένο μέγεθος μπλοκ LZ4 ή Zlib δεν είναι θετικό. |
| NotSupportedException | Οι ρυθμίσεις συμπίεσης λείπουν ή δεν υποστηρίζονται, η άμεση σύνθεση χρησιμοποιεί μια ροή που δεν υποστηρίζει αναζήτηση, ή το μέγεθος της καταχώρισης/αρχείου υπερβαίνει τα τρέχοντα όρια του Apple Archive. |

### Δείτε επίσης

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


