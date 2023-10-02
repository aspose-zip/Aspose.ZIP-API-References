---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: StoreCompressionSettings constructor. Initializes a new instance of the StoreCompressionSettings class
type: docs
weight: 10
url: /net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Initializes a new instance of the [`StoreCompressionSettings`](../) class.

```csharp
public StoreCompressionSettings()
```

## Examples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### See Also

* class [StoreCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../storecompressionsettings/)
* assembly [Aspose.Zip](../../../)


