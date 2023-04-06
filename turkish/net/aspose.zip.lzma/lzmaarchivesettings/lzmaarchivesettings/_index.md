---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: Aspose.ZIP for .NET API Referansı
description: LzmaArchiveSettings inşaatçı. Yeni bir örneğini başlatır.LzmaArchiveSettingsvarsayılan sözlük boyutuna sahip sınıf 16 megabayta eşittir.
type: docs
weight: 10
url: /tr/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Yeni bir örneğini başlatır.[`LzmaArchiveSettings`](../)varsayılan sözlük boyutuna sahip sınıf, 16 megabayta eşittir.

```csharp
public LzmaArchiveSettings()
```

### Örnekler

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### Ayrıca bakınız

* class [LzmaArchiveSettings](../)
* ad alanı [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* toplantı [Aspose.Zip](../../../)


