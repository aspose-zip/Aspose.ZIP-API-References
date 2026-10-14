---
title: "SevenZipEntrySettings.Solid"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "SevenZipEntrySettings özelliği. Girişleri birleştirip tek bir veri bloğu olarak ele alıp almayacağını gösteren bir değeri alır veya ayarlar"
type: docs
weight: 50
url: /tr/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

Girişleri birleştirip tek bir veri bloğu olarak ele alıp almayacağını gösteren değeri alır veya ayarlar.

```csharp
public bool Solid { get; set; }
```

## Açıklamalar

Arşiv oluşturulurken katı 7z arşivi için `SevenZipEntrySettings` sağlayın.

## Örnekler

Aşağıdaki örnek, bir dizini şifreleme olmadan LZMA2 sıkıştırmasıyla katı 7z arşivine nasıl sıkıştıracağınızı gösterir.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### Ayrıca Bakınız

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


