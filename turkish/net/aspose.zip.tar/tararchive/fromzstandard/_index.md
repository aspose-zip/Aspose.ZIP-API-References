---
title: "TarArchive.FromZstandard"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "TarArchive yöntemi. Sağlanan Zstandard arşivini çıkarır ve çıkarılan veriden TarArchive oluşturur"
type: docs
weight: 80
url: /tr/net/aspose.zip.tar/tararchive/fromzstandard/
---
## FromZstandard(Stream) {#fromzstandard}

Sağlanan Zstandard arşivini çıkarır ve çıkarılan veriden [`TarArchive`](../) oluşturur.

Önemli: Zstandard arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

```csharp
public static TarArchive FromZstandard(Stream source)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Akış | Arşivin kaynağı. |

### Dönüş Değeri

Bir [`TarArchive`](../) örneği

### İstisnalar

| istisna | koşul |
| --- | --- |
| IOException | Zstandard akışı bozulmuş veya okunamıyor. |
| InvalidDataException | Veri bozulmuş. |
| EndOfStreamException | Akışın sonuna, beklenen bayt sayısı okunmadan önce ulaşıldığında atılır. |
| ObjectDisposedException | Kaynak akış serbest bırakıldıysa fırlatılır. |

### Ayrıca Bakınız

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZstandard(string) {#fromzstandard_1}

Sağlanan Zstandard arşivini çıkarır ve çıkarılan veriden [`TarArchive`](../) oluşturur.

Önemli: Zstandard arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

```csharp
public static TarArchive FromZstandard(string path)
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
| IOException | Zstandard akışı bozulmuş veya okunamıyor. |
| InvalidDataException | Veri bozulmuş. |
| EndOfStreamException | Akışın sonuna, beklenen bayt sayısı okunmadan önce ulaşıldığında atılır. |

### Ayrıca Bakınız

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


