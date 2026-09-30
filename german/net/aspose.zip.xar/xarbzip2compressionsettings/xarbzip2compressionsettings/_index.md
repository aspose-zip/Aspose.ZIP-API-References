---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "XarBzip2CompressionSettings-Konstruktor. Initialisiert eine neue Instanz der XarBzip2CompressionSettings-Klasse."
type: docs
weight: 10
url: /de/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

Initialisiert eine neue Instanz der [`XarBzip2CompressionSettings`](../)-Klasse.

```csharp
public XarBzip2CompressionSettings(int blockSize)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| blockSize | Int32 | Blockgröße in Hunderten von Kilobytes. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException | Blockgröße liegt nicht zwischen 1 und 9. |

## Beispiele

```csharp
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### Siehe auch

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

Initialisiert eine neue Instanz der [`XarBzip2CompressionSettings`](../)-Klasse mit Standard-Blockgröße, gleich 9 Hundert Kilobyte.

```csharp
public XarBzip2CompressionSettings()
```

### Siehe auch

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


