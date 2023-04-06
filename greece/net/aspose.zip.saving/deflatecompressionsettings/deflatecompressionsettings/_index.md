---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Aspose.ZIP για Αναφορά API .NET
description: DeflateCompressionSettings κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουDeflateCompressionSettings τάξη.
type: docs
weight: 10
url: /el/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Αρχικοποιεί μια νέα παρουσία του[`DeflateCompressionSettings`](../) τάξη.

```csharp
public DeflateCompressionSettings()
```

### Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [DeflateCompressionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* συνέλευση [Aspose.Zip](../../../)


