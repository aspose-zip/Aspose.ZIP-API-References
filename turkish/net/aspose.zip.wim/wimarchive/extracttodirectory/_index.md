---
title: "WimArchive.ExtractToDirectory"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "WimArchive yöntemi. Arşivi belirtilen yola dosya olarak çıkarır"
type: docs
weight: 90
url: /tr/net/aspose.zip.wim/wimarchive/extracttodirectory/
---
## WimArchive.ExtractToDirectory method

Arşivi yola göre dosyaya çıkarır.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationDirectory | String | Çıkarılan dosyaların yerleştirileceği dizinin yolu. |

### Dönüş Değeri

Çıkarılan dosyanın bilgisi.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| ArgumentNullException | *destinationDirectory* null değerindedir |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden kısa ve dosya adları 260 karakterden kısa olmalıdır. |
| SecurityException | Çağıran, mevcut dizine erişmek için gerekli izne sahip değil. |
| NotSupportedException | Dizin mevcut değilse, yol bir sürücü etiketi (\"C:\\") parçası olmayan iki nokta (:) karakteri içerir - veya - WIM arşivi çok parçalıdır. |
| ArgumentException | yol sıfır uzunlukta bir dizedir, yalnızca boşluk içerir veya bir veya daha fazla geçersiz karakter içerir. Geçersiz karakterleri System.IO.Path.GetInvalidPathChars yöntemiyle sorgulayabilirsiniz. -veya- yol yalnızca iki nokta (:) karakteriyle başlar veya onu içerir. |
| IOException | path tarafından belirtilen dizin bir dosyadır. -or- Ağ adı bilinmiyor. |
| InvalidDataException | Arşiv bozulmuş. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |

### Ayrıca Bakınız

* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)


