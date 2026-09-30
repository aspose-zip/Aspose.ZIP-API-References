---
title: "TarArchive.FromLZ4"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "TarArchive yöntemi. Sağlanan LZ4 arşivini çıkarır ve çıkarılan veriden TarArchive oluşturur"
type: docs
weight: 30
url: /tr/net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

Sağlanan LZ4 arşivini çıkarır ve çıkarılan veriden [`TarArchive`](../) oluşturur.

Önemli: LZ4 arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

```csharp
public static TarArchive FromLZ4(string path)
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
| SecurityException | Çağıranın erişim için gerekli izni yok |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya geçersiz bir biçimde. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| FileNotFoundException | Dosya bulunamadı. |
| EndOfStreamException | Dosya çok kısa. |
| InvalidDataException | Dosyanın imzası yanlış. |
| IOException | Dosya açılırken bir G/Ç hatası oluştu. |
| InvalidOperationException | Arşiv birleştirme için hazırlanmıştır. |

## Açıklamalar

LZ4 çıkarma akışı, sıkıştırma algoritmasının doğası gereği arama yapılabilir değildir. Tar arşivi, rastgele kaydı çıkarmak için bir olanak sağlar, bu yüzden altında arama yapılabilir bir akış kullanmak zorundadır.

### Ayrıca Bakınız

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

Sağlanan LZ4 arşivini çıkarır ve çıkarılan veriden [`TarArchive`](../) oluşturur.

Önemli: LZ4 arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

```csharp
public static TarArchive FromLZ4(Stream source)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Akış | Arşivin kaynağı. |

### Dönüş Değeri

Bir [`TarArchive`](../) örneği

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | *source*'dan okunamıyor |
| ArgumentNullException | *source* null. |
| EndOfStreamException | *source* çok kısa. |
| InvalidDataException | *source*'ın imzası yanlış. |
| ObjectDisposedException | Kaynak akış serbest bırakıldıysa fırlatılır. |

## Açıklamalar

LZ4 çıkarma akışı, sıkıştırma algoritmasının doğası gereği arama yapılabilir değildir. Tar arşivi, rastgele kaydı çıkarmak için bir olanak sağlar, bu yüzden altında arama yapılabilir bir akış kullanmak zorundadır.

### Ayrıca Bakınız

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


