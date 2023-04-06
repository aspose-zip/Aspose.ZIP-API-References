---
title: XzCompressionSettings.XzCompressionSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: XzCompressionSettings constructeur. Initialiseert een nieuw exemplaar van hetXzCompressionSettings klasse.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Initialiseert een nieuw exemplaar van het[`XzCompressionSettings`](../) klasse.

```csharp
public XzCompressionSettings()
```

### Voorbeelden

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Zie ook

* class [XzCompressionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../xzcompressionsettings/)
* montage [Aspose.Zip](../../../)


