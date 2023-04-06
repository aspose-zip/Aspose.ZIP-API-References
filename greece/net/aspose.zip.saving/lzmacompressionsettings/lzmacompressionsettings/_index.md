---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Aspose.ZIP για Αναφορά API .NET
description: LzmaCompressionSettings κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουLzmaCompressionSettingsκλάση με προεπιλεγμένο μέγεθος λεξικού ισούται με 16 megabyte.
type: docs
weight: 10
url: /el/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

Αρχικοποιεί μια νέα παρουσία του[`LzmaCompressionSettings`](../)κλάση με προεπιλεγμένο μέγεθος λεξικού, ισούται με 16 megabyte.

```csharp
public LzmaCompressionSettings()
```

### Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [LzmaCompressionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* συνέλευση [Aspose.Zip](../../../)


