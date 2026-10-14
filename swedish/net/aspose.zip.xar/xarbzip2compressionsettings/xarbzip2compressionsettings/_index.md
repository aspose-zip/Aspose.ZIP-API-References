---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Aspose.ZIP för .NET API-referens"
description: "XarBzip2CompressionSettings-constructor. Initierar en ny instans av klassen XarBzip2CompressionSettings."
type: docs
weight: 10
url: /sv/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

Initierar en ny instans av klassen [`XarBzip2CompressionSettings`](../).

```csharp
public XarBzip2CompressionSettings(int blockSize)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blockSize | Int32 | Blockstorlek i hundra kilobyte. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentOutOfRangeException | Blockstorleken är inte mellan 1 och 9. |

## Exempel

```csharp
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### Se även

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

Initierar en ny instans av klassen [`XarBzip2CompressionSettings`](../) med standardblockstorlek, motsvarande 9 hundra kilobyte.

```csharp
public XarBzip2CompressionSettings()
```

### Se även

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


