---
title: "ArjArchive.ArjArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "ArjArchive yapıcı. ArjArchive sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur"
type: docs
weight: 10
url: /tr/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

Yeni bir [`ArjArchive`](../) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| extractionSource | Akış | Arşivin kaynağı. |
| loadOptions | ArjLoadOptions | Mevcut arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *extractionSource* null. |
| ArgumentException | &gt;*extractionSource* aramayı desteklemiyor. |
| InvalidDataException | Arşiv için hatalı imza. - veya - Dosya bir ARJ arşivi değil. |
| EndOfStreamException | Akışın sonuna, tüm başlık baytları veya ad baytları okunmadan önce ulaşıldığında atılır. |
| NotSupportedException | Arşiv bozulmuş. |

## Açıklamalar

Bu yapıcı hiçbir girişi açmaz. Açmak için [`Extract`](../../arjentryplain/extract/) yöntemine bakın.

### Ayrıca Bakınız

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

Yeni bir [`ArjArchive`](../) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Arşiv dosyasının yolu. |
| loadOptions | ArjLoadOptions | Mevcut arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| IOException | Dosya zaten açık. |
| EndOfStreamException | Akışın sonuna, tüm başlık baytları veya ad baytları okunmadan önce ulaşıldığında atılır. |
| InvalidDataException | ARJ sihirli numarası geçersiz veya başlık boyutu aralık dışında. |

## Açıklamalar

Bu yapıcı hiçbir girişi paketlemez. Açmak için [`Extract`](../../arjentryplain/extract/) yöntemine bakın.

## Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ayrıca Bakınız

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


