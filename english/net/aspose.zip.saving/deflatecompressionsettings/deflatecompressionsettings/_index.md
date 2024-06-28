---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: DeflateCompressionSettings constructor. Initializes a new instance of the DeflateCompressionSettings class
type: docs
weight: 10
url: /net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Initializes a new instance of the [`DeflateCompressionSettings`](../) class.

```csharp
public DeflateCompressionSettings()
```

## Examples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### See Also

* class [DeflateCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* assembly [Aspose.Zip](../../../)


