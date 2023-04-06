---
title: XzCompressionSettings.XzCompressionSettings
second_title: Aspose.ZIP for .NET API Referansı
description: XzCompressionSettings inşaatçı. Yeni bir örneğini başlatır.XzCompressionSettings sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Yeni bir örneğini başlatır.[`XzCompressionSettings`](../) sınıf.

```csharp
public XzCompressionSettings()
```

### Örnekler

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Ayrıca bakınız

* class [XzCompressionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../xzcompressionsettings/)
* toplantı [Aspose.Zip](../../../)


