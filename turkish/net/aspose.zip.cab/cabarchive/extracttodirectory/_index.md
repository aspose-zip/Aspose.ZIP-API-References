---
title: CabArchive.ExtractToDirectory
second_title: Aspose.ZIP for .NET API Referansı
description: CabArchive yöntem. Arşivdeki tüm dosyaları sağlanan dizine çıkarır.
type: docs
weight: 40
url: /tr/net/aspose.zip.cab/cabarchive/extracttodirectory/
---
## CabArchive.ExtractToDirectory method

Arşivdeki tüm dosyaları sağlanan dizine çıkarır.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destinationDirectory | String | Ayıklanan dosyaların yerleştirileceği dizinin yolu. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | yol boş |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. |
| SecurityException | Arayan, mevcut dizine erişmek için gerekli izne sahip değil. |
| NotSupportedException | Dizin yoksa yol, sürücü etiketinin ("C:\") parçası olmayan bir iki nokta üst üste karakteri (:) içerir. |
| ArgumentException | yol sıfır uzunluklu bir dizedir, yalnızca boşluk içerir veya bir veya daha fazla geçersiz karakter içerir. System.IO.Path.GetInvalidPathChars yöntemini kullanarak geçersiz karakterleri sorgulayabilirsiniz. -veya- yolun önüne yalnızca bir iki nokta üst üste karakteri (:) eklenir veya içerir. |
| IOException | Yol tarafından belirtilen dizin bir dosyadır. -VEYA- Ağ adı bilinmiyor. |

### Notlar

Dizin yoksa, oluşturulur.

### Örnekler

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ayrıca bakınız

* class [CabArchive](../)
* ad alanı [Aspose.Zip.Cab](../../cabarchive/)
* toplantı [Aspose.Zip](../../../)


