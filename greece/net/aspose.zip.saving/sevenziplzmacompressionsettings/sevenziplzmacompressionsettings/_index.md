---
title: "SevenZipLZMACompressionSettings.SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής SevenZipLZMACompressionSettings. Αρχικοποιεί μια νέα παρουσία της κλάσης SevenZipLZMACompressionSettings με προεπιλεγμένες παραμέτρους."
type: docs
weight: 10
url: /el/net/aspose.zip.saving/sevenziplzmacompressionsettings/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`SevenZipLZMACompressionSettings`](../) με προεπιλεγμένες παραμέτρους.

```csharp
public SevenZipLZMACompressionSettings()
```

## Παραδείγματα

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save("result.7z");
}
```

### Δείτε επίσης

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMACompressionSettings(int, int, int) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`SevenZipLZMACompressionSettings`](../) με καθορισμένο μέγεθος λεξικού, αριθμό γρήγορων byte και αριθμό κυριολεκτικών bits περιβάλλοντος.

```csharp
public SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, 
    int literalContextBits)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dictionarySize | Int32 | Μέγεθος λεξικού (buffer ιστορικού) σε byte. Πρέπει να είναι μεταξύ 4096 και 1073741824, ή ίσο με μηδέν για αυτόματη ανίχνευση βάσει του μεγέθους της καταχώρησης. |
| numberOfFastBytes | Int32 | Ο αριθμός των bytes που χρησιμοποιούνται για γρήγορη αναζήτηση αντιστοιχίας στον αλγόριθμο LZMA. Μπορεί να είναι στο εύρος από 5 έως 273. |
| literalContextBits | Int32 | Ορίζει τον αριθμό των bit περιβάλλοντος κυριολεκτικού (υψηλά bit του προηγούμενου κυριολεκτικού). Μπορεί να είναι στο εύρος από 0 έως 8. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | Εκτοπίζεται όταν κάποιο από τα ορίσματα βρίσκεται εκτός του επιτρεπτού εύρους τιμών. |

### Δείτε επίσης

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMACompressionSettings(int) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`SevenZipLZMACompressionSettings`](../) με καθορισμένο μέγεθος λεξικού, αριθμό γρήγορων byte ίσο με 32 και αριθμό κυριολεκτικών bits περιβάλλοντος ίσο με 3.

```csharp
public SevenZipLZMACompressionSettings(int dictionarySize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dictionarySize | Int32 | Μέγεθος λεξικού (buffer ιστορικού) σε byte. Πρέπει να είναι μεταξύ 4096 και 1073741824, ή ίσο με μηδέν για αυτόματη ανίχνευση βάσει του μεγέθους της καταχώρησης. |

### Δείτε επίσης

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


