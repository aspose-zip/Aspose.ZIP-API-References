---
title: ArchiveLoadOptions.Encoding
second_title: Aspose.ZIP for .NET API Referansı
description: ArchiveLoadOptions mülk. Girdilerin adları için kodlamayı alır veya ayarlar.
type: docs
weight: 30
url: /tr/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Girdilerin adları için kodlamayı alır veya ayarlar.

```csharp
public Encoding Encoding { get; set; }
```

### Örnekler

Zip dosyası özelliklerinden bağımsız olarak belirtilen kodlama kullanılarak oluşturulmuş giriş adı.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### Ayrıca bakınız

* class [ArchiveLoadOptions](../)
* ad alanı [Aspose.Zip](../../archiveloadoptions/)
* toplantı [Aspose.Zip](../../../)


