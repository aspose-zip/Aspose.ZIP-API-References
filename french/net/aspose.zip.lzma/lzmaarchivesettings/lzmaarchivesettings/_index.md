---
title: LzmaArchiveSettings
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Initialise une nouvelle instance duLzmaArchiveSettingsaspose.zip.lzma/lzmaarchivesettings classe avec une taille de dictionnaire par défaut égale à 16 mégaoctets.
type: docs
weight: 10
url: /fr/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Initialise une nouvelle instance du[`LzmaArchiveSettings`](../../lzmaarchivesettings) classe avec une taille de dictionnaire par défaut, égale à 16 mégaoctets.

```csharp
public LzmaArchiveSettings()
```

### Exemples

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### Voir également

* class [LzmaArchiveSettings](../../lzmaarchivesettings)
* espace de noms [Aspose.Zip.LZMA](../../lzmaarchivesettings)
* Assemblée [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->