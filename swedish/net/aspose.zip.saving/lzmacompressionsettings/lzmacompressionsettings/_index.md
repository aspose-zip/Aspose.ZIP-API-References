---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Aspose.ZIP för .NET API-referens
description: LzmaCompressionSettings byggare. Initierar en ny instans avLzmaCompressionSettingsklass med standardstorlek för ordbok lika med 16 megabyte.
type: docs
weight: 10
url: /sv/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

Initierar en ny instans av[`LzmaCompressionSettings`](../)klass med standardstorlek för ordbok, lika med 16 megabyte.

```csharp
public LzmaCompressionSettings()
```

### Exempel

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Se även

* class [LzmaCompressionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* hopsättning [Aspose.Zip](../../../)


