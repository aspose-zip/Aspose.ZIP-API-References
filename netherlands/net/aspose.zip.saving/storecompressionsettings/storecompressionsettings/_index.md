---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: StoreCompressionSettings constructeur. Initialiseert een nieuw exemplaar van hetStoreCompressionSettings klasse.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Initialiseert een nieuw exemplaar van het[`StoreCompressionSettings`](../) klasse.

```csharp
public StoreCompressionSettings()
```

### Voorbeelden

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Zie ook

* class [StoreCompressionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../storecompressionsettings/)
* montage [Aspose.Zip](../../../)


