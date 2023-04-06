---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP για Αναφορά API .NET
description: SevenZipLZMA2CompressionSettings κατασκευαστής. Δημιουργεί τις ρυθμίσεις για τη μέθοδο συμπίεσης LZMA2 εντός αρχείου 7z.
type: docs
weight: 10
url: /el/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Δημιουργεί τις ρυθμίσεις για τη μέθοδο συμπίεσης LZMA2 εντός αρχείου 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dictionarySize | Int32 | Το μέγεθος της προσωρινής μνήμης ιστορικού, πρέπει να είναι μεταξύ 4096 και 1073741824. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* είναι πολύ μεγάλο ή πολύ μικρό. |

### Παρατηρήσεις

Όσο μεγαλύτερο είναι το λεξικό, τόσο καλύτερη είναι συνήθως η αναλογία συμπίεσης, αλλά τα λεξικά μεγαλύτερα από τα ασυμπίεστα δεδομένα είναι σπατάλη μνήμης RAM.

### Δείτε επίσης

* class [SevenZipLZMA2CompressionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* συνέλευση [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Δημιουργεί τις ρυθμίσεις για τη μέθοδο συμπίεσης LZMA2 εντός αρχείου 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dictionarySize | Int32 | Το μέγεθος της προσωρινής μνήμης ιστορικού, πρέπει να είναι μεταξύ 4096 και 1073741824. |
| fastBytes | Int32 | Ελέγχει τον αριθμό των γρήγορων byte που χρησιμοποιούνται από τους συμπιεστές LZMA2. Ένας μεγαλύτερος αριθμός γρήγορων byte μπορεί να προσφέρει καλύτερη αναλογία συμπίεσης σε βάρος της ταχύτητας συμπίεσης. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* είναι πολύ μεγάλο ή πολύ μικρό ή*fastBytes* είναι πολύ μεγάλο ή πολύ μικρό. |

### Παρατηρήσεις

Όσο μεγαλύτερο είναι το λεξικό, τόσο καλύτερη είναι συνήθως η αναλογία συμπίεσης, αλλά τα λεξικά μεγαλύτερα από τα ασυμπίεστα δεδομένα είναι σπατάλη μνήμης RAM.

### Δείτε επίσης

* class [SevenZipLZMA2CompressionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* συνέλευση [Aspose.Zip](../../../)


