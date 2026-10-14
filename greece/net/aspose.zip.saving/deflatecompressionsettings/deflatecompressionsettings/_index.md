---
title: "DeflateCompressionSettings.DeflateCompressionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής DeflateCompressionSettings. Δημιουργεί ένα νέο παράδειγμα της κλάσης DeflateCompressionSettings."
type: docs
weight: 10
url: /el/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Δημιουργεί ένα νέο παράδειγμα της κλάσης [`DeflateCompressionSettings`](../).

```csharp
public DeflateCompressionSettings()
```

## Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [DeflateCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* assembly [Aspose.Zip](../../../)


