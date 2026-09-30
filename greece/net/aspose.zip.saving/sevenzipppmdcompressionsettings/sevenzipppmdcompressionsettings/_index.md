---
title: "SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής SevenZipPPMdCompressionSettings. Δημιουργεί ρυθμίσεις για τη μέθοδο συμπίεσης PPMd μέσα σε αρχείο 7z."
type: docs
weight: 10
url: /el/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Δημιουργεί παραδείγματα ρυθμίσεων για τη μέθοδο συμπίεσης PPMd μέσα σε αρχείο 7z.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| maxOrder | Byte | Μέγιστη τάξη. |
| suballocatorSize | Int32 | Μέγεθος μνήμης σε MB που μπορεί να καταναλώσει ο suballocator. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* δεν είναι μεταξύ 2 και 32, ή *suballocatorSize* δεν είναι μεταξύ 1 και 1024. |

## Παρατηρήσεις

Μεγαλύτερες τάξεις μοντέλου σχεδόν σίγουρα οδηγούν σε καλύτερη συμπίεση και σίγουρα σε μεγαλύτερη χρήση μνήμης και CPU.

Ο αλγόριθμος PPMd μπορεί να χρειάζεται πολύ μνήμη, ειδικά όταν χρησιμοποιείται σε μεγάλα αρχεία και/ή με μεγάλη τάξη μοντέλου. Εάν το ppmd χρειάζεται περισσότερη μνήμη από ό,τι του παρέχετε, η συμπίεση θα είναι χειρότερη.

## Παραδείγματα

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Δείτε επίσης

* class [SevenZipPPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Δημιουργεί παραδείγματα ρυθμίσεων για τη μέθοδο συμπίεσης PPMd μέσα σε αρχείο 7z με προεπιλεγμένη σειρά μοντέλου και μέγεθος υπο-κατανεμητή.

```csharp
public SevenZipPPMdCompressionSettings()
```

## Παρατηρήσεις

Η προεπιλεγμένη τάξη μοντέλου είναι 6 και το μέγεθος του sub-allocator είναι 16 MB.

## Παραδείγματα

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Δείτε επίσης

* class [SevenZipPPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)


