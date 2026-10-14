---
title: "ArjArchive.ExtractToDirectory"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "ArjArchive yöntemi. Tüm girişleri belirtilen dizine çıkarır."
type: docs
weight: 60
url: /tr/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

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
| ArgumentNullException | *destinationDirectory* null olduğunda atılır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| InvalidDataException | Başlıklar veya veri için sağlama toplamı eşleşmiyor. - veya - Arşiv bozulmuş. |
| NotImplementedException | Giriş, yöntem 4 ile sıkıştırılmış. |

## Örnekler

Aşağıdaki örnek, tüm girdileri bir dizine nasıl çıkaracağınızı gösterir:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Ayrıca Bakınız

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


