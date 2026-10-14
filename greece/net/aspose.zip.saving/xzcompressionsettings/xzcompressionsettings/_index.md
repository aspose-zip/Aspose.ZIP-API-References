---
title: "XzCompressionSettings.XzCompressionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής XzCompressionSettings. Αρχικοποιεί μια νέα παρουσία της κλάσης XzCompressionSettings."
type: docs
weight: 10
url: /el/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`XzCompressionSettings`](../).

```csharp
public XzCompressionSettings()
```

## Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [XzCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../xzcompressionsettings/)
* assembly [Aspose.Zip](../../../)


