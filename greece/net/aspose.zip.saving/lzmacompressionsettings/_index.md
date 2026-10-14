---
title: "Κλάση LzmaCompressionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κλάση Aspose.Zip.Saving.LzmaCompressionSettings. Ρυθμίσεις για συμπίεση LZMA εντός αρχείου ZIP."
type: docs
weight: 960
url: /el/net/aspose.zip.saving/lzmacompressionsettings/
---
## LzmaCompressionSettings class

Ρυθμίσεις για τη συμπίεση LZMA μέσα σε ένα αρχείο ZIP.

```csharp
public class LzmaCompressionSettings : CompressionSettings
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor)() | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `LzmaCompressionSettings` με προεπιλεγμένες παραμέτρους. |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor_1)(int) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `LzmaCompressionSettings` με καθορισμένο μέγεθος λεξικού, προεπιλεγμένο αριθμό γρήγορων bytes ίσο με 32 και αριθμό bits κυριολεκτικού πλαισίου ίσο με 3. |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor_2)(int, int, int) | Αρχικοποιεί μια νέα παρουσία της κλάσης `LzmaCompressionSettings` με καθορισμένο μέγεθος λεξικού, αριθμό γρήγορων byte και αριθμό κυριολεκτικών bits περιβάλλοντος. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/lzmacompressionsettings/dictionarysize/) { get; } | Το μέγεθος του λεξικού (buffer ιστορικού) υποδεικνύει πόσα byte των πρόσφατα επεξεργασμένων ασυμπίεστων δεδομένων διατηρούνται στη μνήμη. |
| [LiteralContextBits](../../aspose.zip.saving/lzmacompressionsettings/literalcontextbits/) { get; } | Επιστρέφει τον αριθμό των κυριολεκτικών bits περιβάλλοντος. |
| [NumberOfFastBytes](../../aspose.zip.saving/lzmacompressionsettings/numberoffastbytes/) { get; } | Επιστρέφει τον αριθμό των byte που χρησιμοποιούνται για γρήγορη αναζήτηση αντιστοιχίας στον αλγόριθμο LZMA. |

## Παρατηρήσεις

Ο αλγόριθμος Lempel–Ziv–Markov chain (LZMA) είναι ένας αλγόριθμος που χρησιμοποιείται για την εκτέλεση ασυμπίεστης συμπίεσης δεδομένων. Αυτός ο αλγόριθμος χρησιμοποιεί ένα σχήμα συμπίεσης λεξικού κάπως παρόμοιο με τον αλγόριθμο LZ77 και προσφέρει υψηλό λόγο συμπίεσης και μεταβλητό μέγεθος λεξικού συμπίεσης.

Δείτε περισσότερα: [αλγόριθμος Lempel–Ziv–Markov chain](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### Δείτε επίσης

* class [CompressionSettings](../compressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


