---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: DeflateCompressionSettings constructeur. Initialisiert eine neue Instanz vonDeflateCompressionSettings Klasse.
type: docs
weight: 10
url: /de/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Initialisiert eine neue Instanz von[`DeflateCompressionSettings`](../) Klasse.

```csharp
public DeflateCompressionSettings()
```

### Beispiele

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Siehe auch

* class [DeflateCompressionSettings](../)
* namensraum [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* Montage [Aspose.Zip](../../../)


