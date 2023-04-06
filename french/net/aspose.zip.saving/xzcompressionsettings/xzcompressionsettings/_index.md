---
title: XzCompressionSettings.XzCompressionSettings
second_title: Référence de l'API Aspose.ZIP pour .NET
description: XzCompressionSettings constructeur. Initialise une nouvelle instance duXzCompressionSettings classe.
type: docs
weight: 10
url: /fr/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Initialise une nouvelle instance du[`XzCompressionSettings`](../) classe.

```csharp
public XzCompressionSettings()
```

### Exemples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Voir également

* class [XzCompressionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../xzcompressionsettings/)
* Assemblée [Aspose.Zip](../../../)


