---
title: GzipArchive.Extract
second_title: Aspose.ZIP for .NET API Referansı
description: GzipArchive yöntem. Arşivi sağlanan akışa çıkarır.
type: docs
weight: 40
url: /tr/net/aspose.zip.gzip/gziparchive/extract/
---
## GzipArchive.Extract method

Arşivi sağlanan akışa çıkarır.

```csharp
public void Extract(Stream destination)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destination | Stream | Hedef akışı. Yazılabilir olmalıdır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | *destination* yazmayı desteklemez. |

### Örnekler

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### Ayrıca bakınız

* class [GzipArchive](../)
* ad alanı [Aspose.Zip.Gzip](../../gziparchive/)
* toplantı [Aspose.Zip](../../../)


