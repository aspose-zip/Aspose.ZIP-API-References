---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής XarBzip2CompressionSettings. Αρχικοποιεί μια νέα παρουσία της κλάσης XarBzip2CompressionSettings"
type: docs
weight: 10
url: /el/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`XarBzip2CompressionSettings`](../).

```csharp
public XarBzip2CompressionSettings(int blockSize)
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
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### Δείτε επίσης

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`XarBzip2CompressionSettings`](../) με προεπιλεγμένο μέγεθος μπλοκ, ίσο με 9 εκατοντάδες kilobytes.

```csharp
public XarBzip2CompressionSettings()
```

### Δείτε επίσης

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


