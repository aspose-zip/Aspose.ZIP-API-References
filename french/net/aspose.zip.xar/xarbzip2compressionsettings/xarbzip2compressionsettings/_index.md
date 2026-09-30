---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Constructeur XarBzip2CompressionSettings. Initialise une nouvelle instance de la classe XarBzip2CompressionSettings"
type: docs
weight: 10
url: /fr/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

Initialise une nouvelle instance de la classe [`XarBzip2CompressionSettings`](../).

```csharp
public XarBzip2CompressionSettings(int blockSize)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| blockSize | Int32 | Taille du bloc en centaines de kilooctets. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | La taille du bloc n'est pas comprise entre 1 et 9. |

## Exemples

```csharp
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### Voir aussi

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

Initialise une nouvelle instance de la classe [`XarBzip2CompressionSettings`](../) avec la taille de bloc par défaut, égale à 9 centaines de kilooctets.

```csharp
public XarBzip2CompressionSettings()
```

### Voir aussi

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


