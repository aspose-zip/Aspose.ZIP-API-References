---
title: "ZstandardArchive.Open"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "ZstandardArchive yöntemi. Arşivi çıkarım için açar ve arşiv içeriğiyle bir akış sağlar"
type: docs
weight: 50
url: /tr/net/aspose.zip.zstandard/zstandardarchive/open/
---
## ZstandardArchive.Open method

Arşivi çıkarmak için açar ve arşiv içeriğiyle bir akış sağlar.

```csharp
public Stream Open()
```

### Dönüş Değeri

Arşivin içeriğini temsil eden akış.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Açıklamalar

Bir dosyanın orijinal içeriğini elde etmek için akıştan okuyun. Örnekler bölümüne bakın.

## Örnekler

Arşivi çıkarır ve çıkarılan içeriği dosya akışına kopyalar.

```csharp
using (var archive = new ZstandardArchive("archive.zst"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

.NET 4.0 ve üzeri için Stream.CopyTo yöntemini kullanabilirsiniz:

```csharp
unpacked.CopyTo(extracted);
```

### Ayrıca Bakınız

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


