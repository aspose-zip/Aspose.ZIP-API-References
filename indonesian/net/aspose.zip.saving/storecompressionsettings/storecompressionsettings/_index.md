---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: StoreCompressionSettings konstruktor. Menginisialisasi instance baru dariStoreCompressionSettings kelas.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Menginisialisasi instance baru dari[`StoreCompressionSettings`](../) kelas.

```csharp
public StoreCompressionSettings()
```

### Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Lihat juga

* class [StoreCompressionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../storecompressionsettings/)
* perakitan [Aspose.Zip](../../../)


