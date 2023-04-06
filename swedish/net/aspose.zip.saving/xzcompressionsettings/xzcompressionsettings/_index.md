---
title: XzCompressionSettings.XzCompressionSettings
second_title: Aspose.ZIP för .NET API-referens
description: XzCompressionSettings byggare. Initierar en ny instans avXzCompressionSettings class.
type: docs
weight: 10
url: /sv/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Initierar en ny instans av[`XzCompressionSettings`](../) class.

```csharp
public XzCompressionSettings()
```

### Exempel

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Se även

* class [XzCompressionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../xzcompressionsettings/)
* hopsättning [Aspose.Zip](../../../)


