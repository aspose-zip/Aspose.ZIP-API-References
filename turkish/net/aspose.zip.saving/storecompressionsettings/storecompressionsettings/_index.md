---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Aspose.ZIP for .NET API Referansı
description: StoreCompressionSettings inşaatçı. Yeni bir örneğini başlatır.StoreCompressionSettings sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Yeni bir örneğini başlatır.[`StoreCompressionSettings`](../) sınıf.

```csharp
public StoreCompressionSettings()
```

### Örnekler

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Ayrıca bakınız

* class [StoreCompressionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../storecompressionsettings/)
* toplantı [Aspose.Zip](../../../)


