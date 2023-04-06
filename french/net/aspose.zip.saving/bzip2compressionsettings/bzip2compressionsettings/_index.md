---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Bzip2CompressionSettings constructeur. Initialise une nouvelle instance duBzip2CompressionSettings classe.
type: docs
weight: 10
url: /fr/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

Initialise une nouvelle instance du[`Bzip2CompressionSettings`](../) classe.

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| blockSize | Int32 | Taille de bloc en centaines de kilo-octets. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | La taille du bloc n'est pas comprise entre 1 et 9. |

### Exemples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Voir également

* class [Bzip2CompressionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* Assemblée [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

Initialise une nouvelle instance du[`Bzip2CompressionSettings`](../) classe avec taille de bloc par défaut, égale à 9 centaines de kilo-octets.

```csharp
public Bzip2CompressionSettings()
```

### Exemples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Voir également

* class [Bzip2CompressionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* Assemblée [Aspose.Zip](../../../)


