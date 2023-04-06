---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: Bzip2CompressionSettings constructeur. Initialiseert een nieuw exemplaar van hetBzip2CompressionSettings klasse.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`Bzip2CompressionSettings`](../) klasse.

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| blockSize | Int32 | Blokgrootte in honderden kilobytes. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentOutOfRangeException | Blokgrootte ligt niet tussen 1 en 9. |

### Voorbeelden

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Zie ook

* class [Bzip2CompressionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* montage [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

Initialiseert een nieuw exemplaar van het[`Bzip2CompressionSettings`](../) klasse met standaard blokgrootte, gelijk aan 9 honderd kilobytes.

```csharp
public Bzip2CompressionSettings()
```

### Voorbeelden

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Zie ook

* class [Bzip2CompressionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* montage [Aspose.Zip](../../../)


