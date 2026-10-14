---
title: "SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "SevenZipLZMA2CompressionSettings κατασκευαστής. Δημιουργεί ρυθμίσεις για τη μέθοδο συμπίεσης LZMA2 μέσα σε αρχείο 7z"
type: docs
weight: 10
url: /el/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Δημιουργεί παραδείγματα ρυθμίσεων για τη μέθοδο συμπίεσης LZMA2 μέσα σε αρχείο 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dictionarySize | Int32 | Το μέγεθος του buffer ιστορικού πρέπει να είναι μεταξύ 4096 και 1073741824. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* είναι πολύ μεγάλο ή πολύ μικρό |

## Παρατηρήσεις

Όσο μεγαλύτερο είναι το λεξικό, συνήθως τόσο καλύτερος είναι ο λόγος συμπίεσης - αλλά τα λεξικά μεγαλύτερα από τα ασυμπίεστα δεδομένα είναι σπατάλη μνήμης RAM.

### Δείτε επίσης

* class [SevenZipLZMA2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Δημιουργεί παραδείγματα ρυθμίσεων για τη μέθοδο συμπίεσης LZMA2 μέσα σε αρχείο 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dictionarySize | Int32 | Το μέγεθος του buffer ιστορικού πρέπει να είναι μεταξύ 4096 και 1073741824. |
| fastBytes | Int32 | Ελέγχει τον αριθμό των γρήγορων bytes που χρησιμοποιούν οι συμπιεστές LZMA2. Ένας μεγαλύτερος αριθμός γρήγορων bytes μπορεί να προσφέρει καλύτερο λόγο συμπίεσης με κόστος την ταχύτητα συμπίεσης. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* είναι πολύ μεγάλο ή πολύ μικρό, ή *fastBytes* είναι πολύ μεγάλο ή πολύ μικρό. |

## Παρατηρήσεις

Όσο μεγαλύτερο είναι το λεξικό, συνήθως τόσο καλύτερος είναι ο λόγος συμπίεσης - αλλά τα λεξικά μεγαλύτερα από τα ασυμπίεστα δεδομένα είναι σπατάλη μνήμης RAM.

### Δείτε επίσης

* class [SevenZipLZMA2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assembly [Aspose.Zip](../../../)


