---
title: "StoreCompressionSettings.StoreCompressionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής StoreCompressionSettings. Αρχικοποιεί μια νέα παρουσία της κλάσης StoreCompressionSettings"
type: docs
weight: 10
url: /el/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`StoreCompressionSettings`](../).

```csharp
public StoreCompressionSettings()
```

## Παραδείγματα

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [StoreCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../storecompressionsettings/)
* assembly [Aspose.Zip](../../../)


