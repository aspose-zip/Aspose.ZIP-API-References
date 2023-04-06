---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Aspose.ZIP för .NET API-referens
description: StoreCompressionSettings byggare. Initierar en ny instans avStoreCompressionSettings class.
type: docs
weight: 10
url: /sv/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Initierar en ny instans av[`StoreCompressionSettings`](../) class.

```csharp
public StoreCompressionSettings()
```

### Exempel

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Se även

* class [StoreCompressionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../storecompressionsettings/)
* hopsättning [Aspose.Zip](../../../)


