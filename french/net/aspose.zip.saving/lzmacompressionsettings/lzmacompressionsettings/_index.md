---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Référence de l'API Aspose.ZIP pour .NET
description: LzmaCompressionSettings constructeur. Initialise une nouvelle instance duLzmaCompressionSettingsclasse avec une taille de dictionnaire par défaut égale à 16 mégaoctets.
type: docs
weight: 10
url: /fr/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

Initialise une nouvelle instance du[`LzmaCompressionSettings`](../)classe avec une taille de dictionnaire par défaut, égale à 16 mégaoctets.

```csharp
public LzmaCompressionSettings()
```

### Exemples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Voir également

* class [LzmaCompressionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* Assemblée [Aspose.Zip](../../../)


