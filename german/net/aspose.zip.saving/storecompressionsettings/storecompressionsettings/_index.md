---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: StoreCompressionSettings constructeur. Initialisiert eine neue Instanz vonStoreCompressionSettings Klasse.
type: docs
weight: 10
url: /de/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Initialisiert eine neue Instanz von[`StoreCompressionSettings`](../) Klasse.

```csharp
public StoreCompressionSettings()
```

### Beispiele

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Siehe auch

* class [StoreCompressionSettings](../)
* namensraum [Aspose.Zip.Saving](../../storecompressionsettings/)
* Montage [Aspose.Zip](../../../)


