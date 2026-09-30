---
title: "IsoArchive.ExtractToDirectory"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "IsoArchive yöntemi. Tüm girdileri belirtilen dizine çıkarır."
type: docs
weight: 60
url: /tr/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

Tüm girişleri belirtilen dizine çıkarır.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationDirectory | String | Girdilerin çıkarılacağı dizin. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Arşiv düzenleme modunda olduğunda atılır. |
| ArgumentNullException | *destinationDirectory* null olduğunda atılır. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Örnekler

Aşağıdaki örnek, tüm girdileri bir dizine nasıl çıkaracağınızı gösterir:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Ayrıca Bakınız

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


