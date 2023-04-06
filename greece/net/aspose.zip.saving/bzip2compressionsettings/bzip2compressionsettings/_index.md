---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: Aspose.ZIP για Αναφορά API .NET
description: Bzip2CompressionSettings κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουBzip2CompressionSettings τάξη.
type: docs
weight: 10
url: /el/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`Bzip2CompressionSettings`](../) τάξη.

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| blockSize | Int32 | Μέγεθος μπλοκ σε εκατοντάδες kilobyte. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentOutOfRangeException | Το μέγεθος του μπλοκ δεν είναι μεταξύ 1 και 9. |

### Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [Bzip2CompressionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* συνέλευση [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`Bzip2CompressionSettings`](../) κλάση με προεπιλεγμένο μέγεθος μπλοκ, ισούται με 9 εκατοντάδες kilobyte.

```csharp
public Bzip2CompressionSettings()
```

### Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [Bzip2CompressionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* συνέλευση [Aspose.Zip](../../../)


