---
title: "Bzip2CompressionSettings.Bzip2CompressionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής Bzip2CompressionSettings. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης Bzip2CompressionSettings"
type: docs
weight: 10
url: /el/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Bzip2CompressionSettings`](../).

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| blockSize | Int32 | Μέγεθος μπλοκ σε εκατοντάδες kilobytes. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | Το μέγεθος του τμήματος δεν είναι μεταξύ 1 και 9. |

## Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [Bzip2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Bzip2CompressionSettings`](../) με προεπιλεγμένο μέγεθος τμήματος, ίσο με 9 εκατοντάδες kilobytes.

```csharp
public Bzip2CompressionSettings()
```

## Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [Bzip2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


