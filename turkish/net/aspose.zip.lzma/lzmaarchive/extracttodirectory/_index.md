---
title: "LzmaArchive.ExtractToDirectory"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "LzmaArchive yöntemi. Arşivin içeriğini belirtilen dizine çıkarır"
type: docs
weight: 40
url: /tr/net/aspose.zip.lzma/lzmaarchive/extracttodirectory/
---
## LzmaArchive.ExtractToDirectory method

Arşivin içeriğini sağlanan dizine çıkarır.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationDirectory | String | Çıkarılan dosyaların yerleştirileceği dizinin yolu. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| ArgumentNullException | *destinationDirectory* null. |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden kısa ve dosya adları 260 karakterden kısa olmalıdır. |
| SecurityException | Çağıran, mevcut dizine erişmek için gerekli izne sahip değil. |
| NotSupportedException | Dizin mevcut değilse, yol bir iki nokta üst üste (:) karakteri içerir ve bu, sürücü etiketi (\"C:\\\\"). |
| ArgumentException | *destinationDirectory* sıfır uzunlukta bir dizedir, yalnızca boşluk içerir veya bir veya daha fazla geçersiz karakter içerir. Geçersiz karakterleri sorgulamak için System.IO.Path.GetInvalidPathChars metodunu kullanabilirsiniz. -or- yol yalnızca iki nokta üst üste (:) karakteri ile ön eklenmiş veya sadece bu karakteri içerir. |
| IOException | path tarafından belirtilen dizin bir dosyadır. -or- Ağ adı bilinmiyor. |
| InvalidDataException | Arşiv bozulmuş. |

## Açıklamalar

Dizin mevcut değilse, oluşturulacaktır.

### Ayrıca Bakınız

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)


