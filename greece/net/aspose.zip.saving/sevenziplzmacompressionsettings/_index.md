---
title: "Κλάση SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κλάση Aspose.Zip.Saving.SevenZipLZMACompressionSettings. Ρυθμίσεις για τη μέθοδο συμπίεσης LMA μέσα σε αρχείο 7z"
type: docs
weight: 1090
url: /el/net/aspose.zip.saving/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings class

Ρυθμίσεις για τη μέθοδο συμπίεσης LZMA μέσα σε αρχείο 7z.

```csharp
public class SevenZipLZMACompressionSettings : SevenZipCompressionSettings
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `SevenZipLZMACompressionSettings` με προεπιλεγμένες παραμέτρους. |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor_1)(int) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `SevenZipLZMACompressionSettings` με καθορισμένο μέγεθος λεξικού, αριθμό γρήγορων bytes ίσο με 32, αριθμό bits κυριολεκτικού πλαισίου ίσο με 3. |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor_2)(int, int, int) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `SevenZipLZMACompressionSettings` με καθορισμένο μέγεθος λεξικού, αριθμό γρήγορων bytes και αριθμό bits κυριολεκτικού πλαισίου. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/sevenziplzmacompressionsettings/dictionarysize/) { get; set; } | Το μέγεθος λεξικού (history buffer) υποδεικνύει πόσα bytes των πρόσφατα επεξεργασμένων ασυμπίεστων δεδομένων διατηρούνται στη μνήμη. Εάν δεν οριστεί, θα επιλεγεί ανάλογα με το μέγεθος της εγγραφής. Πρέπει να είναι μεταξύ 4096 και 1073741824, ή ίσο με μηδέν για αυτόματη ανίχνευση βάσει του μεγέθους της εγγραφής. |
| [LiteralContextBits](../../aspose.zip.saving/sevenziplzmacompressionsettings/literalcontextbits/) { get; } | Επιστρέφει τον αριθμό των κυριολεκτικών bits περιβάλλοντος. |
| override [Method](../../aspose.zip.saving/sevenziplzmacompressionsettings/method/) { get; } | Λαμβάνει τη μέθοδο συμπίεσης ή αποσυμπίεσης. |
| [NumberOfFastBytes](../../aspose.zip.saving/sevenziplzmacompressionsettings/numberoffastbytes/) { get; } | Επιστρέφει τον αριθμό των byte που χρησιμοποιούνται για γρήγορη αναζήτηση αντιστοιχίας στον αλγόριθμο LZMA. |

## Παρατηρήσεις

Ο αλγόριθμος Lempel–Ziv–Markov chain (LZMA) είναι ένας αλγόριθμος που χρησιμοποιείται για την εκτέλεση ασυμπίεστης συμπίεσης δεδομένων. Αυτός ο αλγόριθμος χρησιμοποιεί ένα σχήμα συμπίεσης λεξικού κάπως παρόμοιο με τον αλγόριθμο LZ77 και προσφέρει υψηλό λόγο συμπίεσης και μεταβλητό μέγεθος λεξικού συμπίεσης.

Δείτε περισσότερα: [αλγόριθμος Lempel–Ziv–Markov chain](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### Δείτε επίσης

* class [SevenZipCompressionSettings](../sevenzipcompressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


