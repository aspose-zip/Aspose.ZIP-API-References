---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Aspose.ZIP για Αναφορά API .NET
description: SevenZipPPMdCompressionSettings κατασκευαστής. Δημιουργεί τις ρυθμίσεις για τη μέθοδο συμπίεσης PPMd εντός αρχείου 7z.
type: docs
weight: 10
url: /el/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Δημιουργεί τις ρυθμίσεις για τη μέθοδο συμπίεσης PPMd εντός αρχείου 7z.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| maxOrder | Byte | Μέγιστη παραγγελία. |
| suballocatorSize | Int32 | Το μέγεθος μνήμης σε υποκατανομέα MB μπορεί να καταναλώσει. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* δεν είναι μεταξύ 2 και 32 ή*suballocatorSize* δεν είναι μεταξύ 1 και 1024. |

### Παρατηρήσεις

Μεγαλύτερες παραγγελίες μοντέλων σχεδόν σίγουρα έχουν ως αποτέλεσμα καλύτερη συμπίεση και σίγουρα περισσότερη μνήμη και χρήση CPU.

Ο αλγόριθμος PPMd μπορεί να χρειάζεται πολλή μνήμη, ειδικά όταν χρησιμοποιείται σε μεγάλα αρχεία ή/και χρησιμοποιείται με μεγάλη σειρά μοντέλων. Εάν το ppmd χρειάζεται περισσότερη μνήμη από αυτή που του δίνετε, η συμπίεση θα είναι χειρότερη.

### Παραδείγματα

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Δείτε επίσης

* class [SevenZipPPMdCompressionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* συνέλευση [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Δημιουργεί τις ρυθμίσεις για τη μέθοδο συμπίεσης PPMd εντός αρχείου 7z με προεπιλεγμένη σειρά μοντέλου και μέγεθος υποκατανεμητή.

```csharp
public SevenZipPPMdCompressionSettings()
```

### Παρατηρήσεις

Η προεπιλεγμένη παραγγελία μοντέλου είναι 6 και το μέγεθος του δευτερεύοντος εκχωρητή είναι 16 MB.

### Παραδείγματα

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Δείτε επίσης

* class [SevenZipPPMdCompressionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* συνέλευση [Aspose.Zip](../../../)


