---
title: "LzmaArchiveSettings.DictionarySize"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "LzmaArchiveSettings ιδιότητα. Το μέγεθος του buffer ιστορικού λεξικού υποδεικνύει πόσα bytes των πρόσφατα επεξεργασμένων ασυμπίεστων δεδομένων διατηρούνται στη μνήμη. Εάν δεν οριστεί, θα επιλεγεί ανάλογα με το μέγεθος της καταχώρησης"
type: docs
weight: 20
url: /el/net/aspose.zip.lzma/lzmaarchivesettings/dictionarysize/
---
## LzmaArchiveSettings.DictionarySize property

Το μέγεθος του λεξικού (buffer ιστορικού) υποδεικνύει πόσα bytes των πρόσφατα επεξεργασμένων ασυμπίεστων δεδομένων διατηρούνται στη μνήμη. Εάν δεν οριστεί, θα επιλεγεί ανάλογα με το μέγεθος της εγγραφής.

```csharp
public int DictionarySize { get; set; }
```

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | Η τιμή είναι πολύ μικρή ή πολύ μεγάλη. |
| ArgumentException | Η τιμή δεν είναι δύναμη του δύο ή τριπλάσια δύναμη του δύο. |

## Παρατηρήσεις

Όσο μεγαλύτερο είναι το λεξικό, συνήθως τόσο καλύτερος είναι ο λόγος συμπίεσης - αλλά τα λεξικά μεγαλύτερα από τα ασυμπίεστα δεδομένα είναι σπατάλη μνήμης RAM.

Το μέγεθος του λεξικού του αρχείου LZMA πρέπει να είναι είτε δύναμη του δύο (2^n) είτε τριπλάσια δύναμη του δύο (3*2^n).

### Δείτε επίσης

* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


