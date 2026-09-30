---
title: "StoreCompressionSettings.StoreCompressionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor StoreCompressionSettings. Menginisialisasi sebuah instance baru dari kelas StoreCompressionSettings"
type: docs
weight: 10
url: /id/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Menginisialisasi sebuah instance baru dari kelas [`StoreCompressionSettings`](../).

```csharp
public StoreCompressionSettings()
```

## Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Lihat Juga

* class [StoreCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../storecompressionsettings/)
* assembly [Aspose.Zip](../../../)


