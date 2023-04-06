---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Aspose.ZIP for .NET API Referansı
description: LzmaCompressionSettings inşaatçı. Yeni bir örneğini başlatır.LzmaCompressionSettingsvarsayılan sözlük boyutuna sahip sınıf 16 megabayta eşittir.
type: docs
weight: 10
url: /tr/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

Yeni bir örneğini başlatır.[`LzmaCompressionSettings`](../)varsayılan sözlük boyutuna sahip sınıf, 16 megabayta eşittir.

```csharp
public LzmaCompressionSettings()
```

### Örnekler

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Ayrıca bakınız

* class [LzmaCompressionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* toplantı [Aspose.Zip](../../../)


