---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Référence de l'API Aspose.ZIP pour .NET
description: XzBcjX86FilterSettings constructeur. Initialise une nouvelle instance duXzBcjX86FilterSettings . Utilisezle pour compresser des fichiers exécutables et des bibliothèques dansXzArchive .
type: docs
weight: 10
url: /fr/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

Initialise une nouvelle instance du[`XzBcjX86FilterSettings`](../) . Utilisez-le pour compresser des fichiers exécutables et des bibliothèques dans[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### Exemples

```csharp
XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
using (XzArchive archive = new XzArchive(settings))
{
    archive.SetSource("data.bin");
    archive.Save("archive.xz");
}
```

### Voir également

* class [XzBcjX86FilterSettings](../)
* espace de noms [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* Assemblée [Aspose.Zip](../../../)


