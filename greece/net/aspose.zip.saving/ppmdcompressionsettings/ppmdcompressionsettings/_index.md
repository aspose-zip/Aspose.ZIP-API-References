---
title: PPMdCompressionSettings.PPMdCompressionSettings
second_title: Aspose.ZIP για Αναφορά API .NET
description: PPMdCompressionSettings κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουPPMdCompressionSettings τάξη.
type: docs
weight: 10
url: /el/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`PPMdCompressionSettings`](../) τάξη.

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| modelOrder | Int32 | Παραγγελία του μοντέλου. |
| suballocatorSize | Int32 | Το μέγεθος μνήμης σε υποκατανομέα MB μπορεί να καταναλώσει. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* δεν είναι μεταξύ 2 και 16. - ή -*suballocatorSize* δεν είναι μεταξύ 1 και 256. |

### Παρατηρήσεις

Μεγαλύτερες παραγγελίες μοντέλων σχεδόν σίγουρα έχουν ως αποτέλεσμα καλύτερη συμπίεση και σίγουρα περισσότερη μνήμη και χρήση CPU.

Ο αλγόριθμος PPMd μπορεί να χρειάζεται πολλή μνήμη, ειδικά όταν χρησιμοποιείται σε μεγάλα αρχεία ή/και χρησιμοποιείται με μεγάλη σειρά μοντέλων. Εάν το ppmd χρειάζεται περισσότερη μνήμη από αυτή που του δίνετε, η συμπίεση θα είναι χειρότερη.

### Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [PPMdCompressionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* συνέλευση [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`PPMdCompressionSettings`](../) κλάση με προεπιλεγμένη σειρά μοντέλου και μέγεθος υποκατανεμητή.

```csharp
public PPMdCompressionSettings()
```

### Παρατηρήσεις

Η προεπιλεγμένη παραγγελία μοντέλου είναι 8 και το μέγεθος του δευτερεύοντος εκχωρητή είναι 50 MB.

### Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [PPMdCompressionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* συνέλευση [Aspose.Zip](../../../)


