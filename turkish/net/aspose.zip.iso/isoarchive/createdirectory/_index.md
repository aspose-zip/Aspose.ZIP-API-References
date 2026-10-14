---
title: "IsoArchive.CreateDirectory"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "IsoArchive yöntemi. ISO görüntüsüne bir dizin ekler"
type: docs
weight: 30
url: /tr/net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

ISO görüntüsüne bir dizin ekler.

```csharp
public IsoEntry CreateDirectory(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | ISO içindeki dizinin yolu. |

### Dönüş Değeri

ISO girişi oluşturuldu.

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Arşiv çıkarma için açıldı. |
| ArgumentNullException | `name` null veya boş. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

### Ayrıca Bakınız

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


