---
title: Bzip2Archive.Extract
second_title: Aspose.ZIP for .NET API Referansı
description: Bzip2Archive yöntem. Arşivi sağlanan akışa çıkarır.
type: docs
weight: 30
url: /tr/net/aspose.zip.bzip2/bzip2archive/extract/
---
## Bzip2Archive.Extract method

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
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### Ayrıca bakınız

* class [Bzip2Archive](../)
* ad alanı [Aspose.Zip.Bzip2](../../bzip2archive/)
* toplantı [Aspose.Zip](../../../)


