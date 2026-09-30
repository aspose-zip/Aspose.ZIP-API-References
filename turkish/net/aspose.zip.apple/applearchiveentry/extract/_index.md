---
title: "AppleArchiveEntry.Extract"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "AppleArchiveEntry yöntemi. Sağlanan yola göre girişi dosya sistemine çıkarır"
type: docs
weight: 50
url: /tr/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

Girişi sağlanan yola göre dosya sistemine çıkarır.

```csharp
public FileInfo Extract(string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidDataException | Girdi için saklanan sağlama toplamı veya özet, çıkarılan verilerle eşleşmiyor. |
| InvalidOperationException | Girdi, birleştirme için hazırlanmış bir arşive aittir veya giriş verileri aranamaz bir arşiv akışından açılamaz. |
| NotSupportedException | Girdi, katı bir Apple Arşivi'ne aittir veya desteklenmeyen bir sıkıştırma yöntemi kullanır. |
| ObjectDisposedException | Kaynak akış iptal edildi. |
| IOException | Bir G/Ç hatası oluştu. |

### Ayrıca Bakınız

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Girişi sağlanan akışa çıkarır.

```csharp
public void Extract(Stream destination)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | Akış | Hedef akış. Yazılabilir olmalıdır. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *destination* `null`'dır. |
| ArgumentException | *destination* yazmayı desteklemiyor. |
| InvalidDataException | Girdi için saklanan sağlama toplamı veya özet, çıkarılan verilerle eşleşmiyor. |
| InvalidOperationException | Girdi, birleştirme için hazırlanmış bir arşive aittir veya giriş verileri aranamaz bir arşiv akışından açılamaz. |
| NotSupportedException | Girdi, katı bir Apple Arşivi'ne aittir veya desteklenmeyen bir sıkıştırma yöntemi kullanır. |
| ObjectDisposedException | Kaynak akış iptal edildi. |
| IOException | Bir G/Ç hatası oluştu. |

### Ayrıca Bakınız

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


