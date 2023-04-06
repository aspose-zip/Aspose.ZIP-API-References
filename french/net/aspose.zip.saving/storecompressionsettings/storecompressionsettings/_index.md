---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Référence de l'API Aspose.ZIP pour .NET
description: StoreCompressionSettings constructeur. Initialise une nouvelle instance duStoreCompressionSettings classe.
type: docs
weight: 10
url: /fr/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Initialise une nouvelle instance du[`StoreCompressionSettings`](../) classe.

```csharp
public StoreCompressionSettings()
```

### Exemples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Voir également

* class [StoreCompressionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../storecompressionsettings/)
* Assemblée [Aspose.Zip](../../../)


