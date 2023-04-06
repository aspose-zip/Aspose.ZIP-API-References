---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP for .NET API Referansı
description: SevenZipLZMA2CompressionSettings inşaatçı. 7z arşivi içinde LZMA2 sıkıştırma yöntemi için ayarları somutlaştırır.
type: docs
weight: 10
url: /tr/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

7z arşivi içinde LZMA2 sıkıştırma yöntemi için ayarları somutlaştırır.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| dictionarySize | Int32 | Geçmiş arabelleğinin boyutu, 4096 ile 1073741824 arasında olmalıdır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* çok büyük veya çok küçük. |

### Notlar

Sözlük ne kadar büyükse, sıkıştırma oranı genellikle o kadar iyidir, ancak sıkıştırılmamış verilerden daha büyük sözlükler RAM israfına neden olur.

### Ayrıca bakınız

* class [SevenZipLZMA2CompressionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* toplantı [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

7z arşivi içinde LZMA2 sıkıştırma yöntemi için ayarları somutlaştırır.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| dictionarySize | Int32 | Geçmiş arabelleğinin boyutu, 4096 ile 1073741824 arasında olmalıdır. |
| fastBytes | Int32 | LZMA2 kompresörleri tarafından kullanılan hızlı bayt sayısını kontrol eder. Daha fazla sayıda hızlı bayt, sıkıştırma hızı pahasına daha iyi bir sıkıştırma oranı sağlayabilir. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* çok büyük veya çok küçük veya*fastBytes* çok büyük veya çok küçük. |

### Notlar

Sözlük ne kadar büyükse, sıkıştırma oranı genellikle o kadar iyidir, ancak sıkıştırılmamış verilerden daha büyük sözlükler RAM israfına neden olur.

### Ayrıca bakınız

* class [SevenZipLZMA2CompressionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* toplantı [Aspose.Zip](../../../)


