---
title: "LzmaCompressionSettings.LzmaCompressionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής LzmaCompressionSettings. Αρχικοποιεί μια νέα παρουσία της κλάσης LzmaCompressionSettings με προεπιλεγμένες παραμέτρους."
type: docs
weight: 10
url: /el/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LzmaCompressionSettings`](../) με προεπιλεγμένες παραμέτρους.

```csharp
public LzmaCompressionSettings()
```

## Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## LzmaCompressionSettings(int, int, int) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`LzmaCompressionSettings`](../) με καθορισμένο μέγεθος λεξικού, αριθμό γρήγορων bytes και αριθμό bits κυριολεκτικού πλαισίου.

```csharp
public LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dictionarySize | Int32 | Μέγεθος λεξικού (buffer ιστορικού) σε bytes. Πρέπει να είναι μεταξύ 4096 και 1073741824. |
| numberOfFastBytes | Int32 | Ο αριθμός των bytes που χρησιμοποιούνται για γρήγορη αναζήτηση αντιστοιχίας στον αλγόριθμο LZMA. Μπορεί να είναι στο εύρος από 5 έως 273. |
| literalContextBits | Int32 | Ορίζει τον αριθμό των bit περιβάλλοντος κυριολεκτικού (υψηλά bit του προηγούμενου κυριολεκτικού). Μπορεί να είναι στο εύρος από 0 έως 8. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | Εκτοπίζεται όταν κάποιο από τα ορίσματα βρίσκεται εκτός του επιτρεπτού εύρους τιμών. |

### Δείτε επίσης

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## LzmaCompressionSettings(int) {#constructor_1}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`LzmaCompressionSettings`](../) με καθορισμένο μέγεθος λεξικού, προεπιλεγμένο αριθμό γρήγορων byte ίσο με 32 και αριθμό bit περιβάλλοντος κυριολεκτικού ίσο με 3.

```csharp
public LzmaCompressionSettings(int dictionarySize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dictionarySize | Int32 | Μέγεθος λεξικού (buffer ιστορικού) σε bytes. Πρέπει να είναι μεταξύ 4096 και 1073741824. |

### Δείτε επίσης

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


