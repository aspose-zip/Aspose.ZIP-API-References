---
title: "LhaArchive.ExtractToDirectory"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "LhaArchive yöntemi. Arşivdeki tüm dosya ve dizinleri verilen dizine çıkarır"
type: docs
weight: 40
url: /tr/net/aspose.zip.lha/lhaarchive/extracttodirectory/
---
## LhaArchive.ExtractToDirectory method

Arşivdeki tüm dosya ve dizinleri verilen dizine çıkarır.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationDirectory | String | Çıkarılan dosyaların yerleştirileceği dizinin yolu. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *destinationDirectory* null. |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden kısa ve dosya adları 260 karakterden kısa olmalıdır. |
| SecurityException | Çağıran, mevcut dizine erişmek için gerekli izne sahip değil. |
| NotSupportedException | Dizin mevcut değilse, yol bir iki nokta üst üste (:) karakteri içerir ve bu, sürücü etiketi (\"C:\\\\"). |
| ArgumentException | *destinationDirectory* sıfır uzunlukta bir dizedir, yalnızca boşluk içerir veya bir veya daha fazla geçersiz karakter içerir. Geçersiz karakterleri sorgulamak için System.IO.Path.GetInvalidPathChars metodunu kullanabilirsiniz. -or- yol yalnızca iki nokta üst üste (:) karakteri ile ön eklenmiş veya sadece bu karakteri içerir. |
| IOException | path tarafından belirtilen dizin bir dosyadır. -or- Ağ adı bilinmiyor. |
| InvalidDataException | Yanlış şifre girildi. - veya - Arşiv bozuk. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| ObjectDisposedException | Nesne atıldıktan sonra (dispose edildiğinde) fırlatılır. |

## Açıklamalar

Dizin mevcut değilse, oluşturulacaktır.

## Örnekler

```csharp
using (var archive = new LhaArchive("archive.lzh")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ayrıca Bakınız

* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


