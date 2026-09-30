---
title: "Lz4Archive.Open"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Lz4Archive yöntemi. Arşivi çıkarma için açar ve arşiv içeriğiyle bir akış sağlar"
type: docs
weight: 50
url: /tr/net/aspose.zip.lz4/lz4archive/open/
---
## Lz4Archive.Open method

Arşivi çıkarmak için açar ve arşiv içeriğiyle bir akış sağlar.

```csharp
public Stream Open()
```

### Dönüş Değeri

Arşivin içeriğini temsil eden akış.

### İstisnalar

| istisna | koşul |
| --- | --- |
| EndOfStreamException | Kaynak akış çok kısadır. |
| InvalidDataException | Kod çözme başlatılırken hatalı baytlar bulundu. |
| InvalidOperationException | Arşiv birleştirme için hazırlanmıştır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| IOException | Bir G/Ç hatası oluştu. |

## Açıklamalar

Bir dosyanın orijinal içeriğini elde etmek için akıştan okuyun. Örnekler bölümüne bakın.

## Örnekler

Arşivi çıkarır ve çıkarılan içeriği dosya akışına kopyalar.

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
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

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


