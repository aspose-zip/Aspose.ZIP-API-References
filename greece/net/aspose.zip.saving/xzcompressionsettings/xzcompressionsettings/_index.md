---
title: XzCompressionSettings.XzCompressionSettings
second_title: Aspose.ZIP για Αναφορά API .NET
description: XzCompressionSettings κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουXzCompressionSettings τάξη.
type: docs
weight: 10
url: /el/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Αρχικοποιεί μια νέα παρουσία του[`XzCompressionSettings`](../) τάξη.

```csharp
public XzCompressionSettings()
```

### Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [XzCompressionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../xzcompressionsettings/)
* συνέλευση [Aspose.Zip](../../../)


