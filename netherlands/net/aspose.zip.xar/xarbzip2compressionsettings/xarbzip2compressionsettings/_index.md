---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "XarBzip2CompressionSettings constructor. Initialiseert een nieuw exemplaar van de XarBzip2CompressionSettings-klasse"
type: docs
weight: 10
url: /nl/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`XarBzip2CompressionSettings`](../) klasse.

```csharp
public XarBzip2CompressionSettings(int blockSize)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| blockSize | Int32 | Blokgrootte in honderden kilobytes. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentOutOfRangeException | Blokgrootte is niet tussen 1 en 9. |

## Voorbeelden

```csharp
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### Zie ook

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

Initialiseert een nieuw exemplaar van de [`XarBzip2CompressionSettings`](../) klasse met de standaard blokgrootte, gelijk aan 9 honderd kilobytes.

```csharp
public XarBzip2CompressionSettings()
```

### Zie ook

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


