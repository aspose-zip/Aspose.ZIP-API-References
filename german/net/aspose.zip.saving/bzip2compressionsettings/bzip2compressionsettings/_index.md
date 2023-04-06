---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: Bzip2CompressionSettings constructeur. Initialisiert eine neue Instanz vonBzip2CompressionSettings Klasse.
type: docs
weight: 10
url: /de/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

Initialisiert eine neue Instanz von[`Bzip2CompressionSettings`](../) Klasse.

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| blockSize | Int32 | Blockgröße in Hunderten von Kilobyte. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException | Die Blockgröße liegt nicht zwischen 1 und 9. |

### Beispiele

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Siehe auch

* class [Bzip2CompressionSettings](../)
* namensraum [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* Montage [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

Initialisiert eine neue Instanz von[`Bzip2CompressionSettings`](../) Klasse mit Standardblockgröße, entspricht 900 Kilobyte.

```csharp
public Bzip2CompressionSettings()
```

### Beispiele

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Siehe auch

* class [Bzip2CompressionSettings](../)
* namensraum [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* Montage [Aspose.Zip](../../../)


