---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: LzmaCompressionSettings constructeur. Initialisiert eine neue Instanz vonLzmaCompressionSettingsKlasse mit Standardwörterbuchgröße entspricht 16 Megabyte.
type: docs
weight: 10
url: /de/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

Initialisiert eine neue Instanz von[`LzmaCompressionSettings`](../)Klasse mit Standardwörterbuchgröße, entspricht 16 Megabyte.

```csharp
public LzmaCompressionSettings()
```

### Beispiele

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Siehe auch

* class [LzmaCompressionSettings](../)
* namensraum [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* Montage [Aspose.Zip](../../../)


