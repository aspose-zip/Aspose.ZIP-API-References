---
title: XzCompressionSettings.XzCompressionSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: XzCompressionSettings constructeur. Initialisiert eine neue Instanz vonXzCompressionSettings Klasse.
type: docs
weight: 10
url: /de/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Initialisiert eine neue Instanz von[`XzCompressionSettings`](../) Klasse.

```csharp
public XzCompressionSettings()
```

### Beispiele

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Siehe auch

* class [XzCompressionSettings](../)
* namensraum [Aspose.Zip.Saving](../../xzcompressionsettings/)
* Montage [Aspose.Zip](../../../)


