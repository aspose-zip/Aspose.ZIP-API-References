---
title: "PPMdCompressionSettings.PPMdCompressionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "PPMdCompressionSettings κατασκευαστής. Αρχικοποιεί μια νέα παρουσία της κλάσης PPMdCompressionSettings"
type: docs
weight: 10
url: /el/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PPMdCompressionSettings`](../).

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| modelOrder | Int32 | Σειρά του μοντέλου. |
| suballocatorSize | Int32 | Μέγεθος μνήμης σε MB που μπορεί να καταναλώσει ο suballocator. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* δεν είναι μεταξύ 2 και 16. - ή - *suballocatorSize* δεν είναι μεταξύ 1 και 256. |

## Παρατηρήσεις

Μεγαλύτερες τάξεις μοντέλου σχεδόν σίγουρα οδηγούν σε καλύτερη συμπίεση και σίγουρα σε μεγαλύτερη χρήση μνήμης και CPU.

Ο αλγόριθμος PPMd μπορεί να χρειάζεται πολύ μνήμη, ειδικά όταν χρησιμοποιείται σε μεγάλα αρχεία και/ή με μεγάλη τάξη μοντέλου. Εάν το ppmd χρειάζεται περισσότερη μνήμη από ό,τι του παρέχετε, η συμπίεση θα είναι χειρότερη.

## Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [PPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PPMdCompressionSettings`](../) με προεπιλεγμένη σειρά μοντέλου και μέγεθος υπο-διανεμητή.

```csharp
public PPMdCompressionSettings()
```

## Παρατηρήσεις

Η προεπιλεγμένη σειρά μοντέλου είναι 8 και το μέγεθος υπο-διανεμητή είναι 50MB.

## Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [PPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)


