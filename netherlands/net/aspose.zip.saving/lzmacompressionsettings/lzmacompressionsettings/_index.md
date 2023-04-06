---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: LzmaCompressionSettings constructeur. Initialiseert een nieuw exemplaar van hetLzmaCompressionSettingsklasse met standaard woordenboekgrootte gelijk aan 16 megabytes.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

Initialiseert een nieuw exemplaar van het[`LzmaCompressionSettings`](../)klasse met standaard woordenboekgrootte, gelijk aan 16 megabytes.

```csharp
public LzmaCompressionSettings()
```

### Voorbeelden

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Zie ook

* class [LzmaCompressionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* montage [Aspose.Zip](../../../)


