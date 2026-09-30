---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "AlzArchiveLoadOptions özelliği. Giriş adları için kodlamayı alır veya ayarlar. Varsayılan Kore Windows kod sayfası 949 CP949'tir."
type: docs
weight: 40
url: /tr/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

Giriş adlarının kodlamasını alır veya ayarlar. Varsayılan, Kore Windows kod sayfası 949 (CP949)'dur.

```csharp
public Encoding Encoding { get; set; }
```

## Açıklamalar

ALZ arşivleri tarihsel olarak dosya adlarını Kore Windows ANSI kod sayfasını kullanarak depolar.

## Örnekler

Giriş adı belirtilen kodlama kullanılarak oluşturulur.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### Ayrıca Bakınız

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


