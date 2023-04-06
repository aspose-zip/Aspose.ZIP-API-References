---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: DeflateCompressionSettings constructeur. Initialiseert een nieuw exemplaar van hetDeflateCompressionSettings klasse.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Initialiseert een nieuw exemplaar van het[`DeflateCompressionSettings`](../) klasse.

```csharp
public DeflateCompressionSettings()
```

### Voorbeelden

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Zie ook

* class [DeflateCompressionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* montage [Aspose.Zip](../../../)


