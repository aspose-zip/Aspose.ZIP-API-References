---
title: XzCompressionSettings.XzCompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: XzCompressionSettings constructor. Initializes a new instance of the XzCompressionSettings class
type: docs
weight: 10
url: /net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Initializes a new instance of the [`XzCompressionSettings`](../) class.

```csharp
public XzCompressionSettings()
```

## Examples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### See Also

* class [XzCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../xzcompressionsettings/)
* assembly [Aspose.Zip](../../../)


