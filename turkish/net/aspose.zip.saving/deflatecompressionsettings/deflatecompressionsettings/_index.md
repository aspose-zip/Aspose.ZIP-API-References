---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Aspose.ZIP for .NET API Referansı
description: DeflateCompressionSettings inşaatçı. Yeni bir örneğini başlatır.DeflateCompressionSettings sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Yeni bir örneğini başlatır.[`DeflateCompressionSettings`](../) sınıf.

```csharp
public DeflateCompressionSettings()
```

### Örnekler

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Ayrıca bakınız

* class [DeflateCompressionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* toplantı [Aspose.Zip](../../../)


