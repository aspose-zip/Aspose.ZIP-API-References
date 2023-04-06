---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Référence de l'API Aspose.ZIP pour .NET
description: DeflateCompressionSettings constructeur. Initialise une nouvelle instance duDeflateCompressionSettings classe.
type: docs
weight: 10
url: /fr/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Initialise une nouvelle instance du[`DeflateCompressionSettings`](../) classe.

```csharp
public DeflateCompressionSettings()
```

### Exemples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Voir également

* class [DeflateCompressionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* Assemblée [Aspose.Zip](../../../)


