---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Aspose.ZIP för .NET API-referens
description: DeflateCompressionSettings byggare. Initierar en ny instans avDeflateCompressionSettings class.
type: docs
weight: 10
url: /sv/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Initierar en ny instans av[`DeflateCompressionSettings`](../) class.

```csharp
public DeflateCompressionSettings()
```

### Exempel

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Se även

* class [DeflateCompressionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* hopsättning [Aspose.Zip](../../../)


