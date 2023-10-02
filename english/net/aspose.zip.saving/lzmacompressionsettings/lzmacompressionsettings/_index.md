---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: LzmaCompressionSettings constructor. Initializes a new instance of the LzmaCompressionSettings class with default dictionary size equals to 16 megabytes
type: docs
weight: 10
url: /net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

Initializes a new instance of the [`LzmaCompressionSettings`](../) class with default dictionary size, equals to 16 megabytes.

```csharp
public LzmaCompressionSettings()
```

## Examples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### See Also

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


