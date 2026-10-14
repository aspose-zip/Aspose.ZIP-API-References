---
title: "Lz4Archive.ExtractToDirectory"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Lz4Archive yöntemi. Arşivin içeriğini belirtilen dizine çıkarır"
type: docs
weight: 40
url: /tr/net/aspose.zip.lz4/lz4archive/extracttodirectory/
---
## Lz4Archive.ExtractToDirectory method

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
| ArgumentNullException | *destinationDirectory* null. |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden kısa ve dosya adları 260 karakterden kısa olmalıdır. |
| SecurityException | Çağıran, mevcut dizine erişmek için gerekli izne sahip değil. |
| NotSupportedException | Dizin mevcut değilse, yol bir iki nokta üst üste (:) karakteri içerir ve bu, sürücü etiketi (\"C:\\\\"). |
| ArgumentException | *destinationDirectory* sıfır uzunlukta bir dizedir, yalnızca boşluk içerir veya bir veya daha fazla geçersiz karakter içerir. Geçersiz karakterleri sorgulamak için System.IO.Path.GetInvalidPathChars metodunu kullanabilirsiniz. -or- yol yalnızca iki nokta üst üste (:) karakteri ile ön eklenmiş veya sadece bu karakteri içerir. |
| IOException | path tarafından belirtilen dizin bir dosyadır. -or- Ağ adı bilinmiyor. |
| EndOfStreamException | Kaynak akış çok kısadır. |
| InvalidDataException | Kod çözme başlatılırken hatalı baytlar bulundu. |
| InvalidOperationException | Arşiv birleştirme için hazırlanmıştır. |
| OperationCanceledException | .NET Framework 4.0 ve üzeri: Çıkarma, sağlanan iptal belirteciyle iptal edildiğinde atılır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Açıklamalar

Dizin mevcut değilse, oluşturulacaktır.

### Ayrıca Bakınız

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


