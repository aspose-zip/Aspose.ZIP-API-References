---
title: "Κλάση SevenZipCipher"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κλάση Aspose.Zip.Crypto.SevenZipCipher. Βασική κλάση για τον κρυπτογράφο AES που χρησιμοποιείται για την κρυπτογράφηση 7zip"
type: docs
weight: 440
url: /el/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

Βασική κλάση για τον κρυπτογράφο AES που χρησιμοποιείται για την κρυπτογράφηση 7-zip.

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν η τρέχουσα μετατροπή μπορεί να επαναχρησιμοποιηθεί. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν μπορούν να μετατραπούν πολλαπλά μπλοκ. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | Λαμβάνει το μέγεθος του μπλοκ εισόδου. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | Λαμβάνει το μέγεθος του μπλοκ εξόδου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | Εκτελεί εργασίες ορισμένες από την εφαρμογή που σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | Μετατρέπει την καθορισμένη περιοχή του πίνακα byte εισόδου και αντιγράφει τη δημιουργημένη μετατροπή στην καθορισμένη περιοχή του πίνακα byte εξόδου. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | Μετατρέπει την καθορισμένη περιοχή του καθορισμένου πίνακα byte. |

### Δείτε επίσης

* namespace [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* assembly [Aspose.Zip](../../)


