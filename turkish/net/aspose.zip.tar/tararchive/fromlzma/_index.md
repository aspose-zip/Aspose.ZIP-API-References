---
title: "TarArchive.FromLZMA"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "TarArchive yöntemi. Sağlanan LZMA arşivini çıkarır ve çıkarılan veriden TarArchive oluşturur"
type: docs
weight: 50
url: /tr/net/aspose.zip.tar/tararchive/fromlzma/
---
## FromLZMA(Stream) {#fromlzma}

Sağlanan LZMA arşivini çıkarır ve çıkarılan veriden [`TarArchive`](../) oluşturur.

Önemli: LZMA arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

```csharp
public static TarArchive FromLZMA(Stream source)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Akış | Arşivin kaynağı. |

### Dönüş Değeri

Bir [`TarArchive`](../) örneği

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidDataException | Arşiv bozulmuş. |
| EndOfStreamException | Akışın sonuna, beklenen bayt sayısı okunmadan önce ulaşıldığında atılır. |
| ObjectDisposedException | Kaynak akış serbest bırakıldıysa fırlatılır. |
| ArgumentNullException | *source* null. |
| IOException | Bir G/Ç hatası oluştu. |

## Açıklamalar

LZMA çıkarma akışı, sıkıştırma algoritmasının doğası gereği aranabilir değildir. Tar arşivi, rastgele kaydı çıkarmak için bir kolaylık sağlar, bu yüzden altında aranabilir bir akış kullanmak zorundadır.

### Ayrıca Bakınız

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZMA(string) {#fromlzma_1}

Sağlanan LZMA arşivini çıkarır ve çıkarılan veriden [`TarArchive`](../) oluşturur.

Önemli: LZMA arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

```csharp
public static TarArchive FromLZMA(string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Arşiv dosyasının yolu. |

### Dönüş Değeri

Bir [`TarArchive`](../) örneği

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya geçersiz bir biçimde. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| FileNotFoundException | Dosya bulunamadı. |
| EndOfStreamException | Akışın sonuna, beklenen bayt sayısı okunmadan önce ulaşıldığında atılır. |
| IOException | Dosya açılırken bir G/Ç hatası oluştu. |
| InvalidDataException | Arşiv bozulmuş. |

## Açıklamalar

LZMA çıkarma akışı, sıkıştırma algoritmasının doğası gereği aranabilir değildir. Tar arşivi, rastgele kaydı çıkarmak için bir kolaylık sağlar, bu yüzden altında aranabilir bir akış kullanmak zorundadır.

### Ayrıca Bakınız

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


