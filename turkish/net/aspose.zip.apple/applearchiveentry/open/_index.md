---
title: "AppleArchiveEntry.Open"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "AppleArchiveEntry yöntemi. Girdiyi çıkarma için açar ve girdinin içeriğini sağlayan bir akış sunar."
type: docs
weight: 60
url: /tr/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

Girdiyi çıkarmak için açar ve girdinin içeriğini içeren bir akış sağlar

```csharp
public Stream Open()
```

### Dönüş Değeri

Çıkarılan giriş verilerini içeren okunabilir bir akış.

### İstisnalar

| istisna | koşul |
| --- | --- |
| NotSupportedException | Girdi, katı bir Apple Arşivi'ne aittir veya desteklenmeyen bir sıkıştırma yöntemi kullanır. |
| InvalidDataException | Girdi için saklanan sağlama toplamı veya özet, çıkarılan verilerle eşleşmiyor. |
| InvalidOperationException | Girdi, birleştirme için hazırlanmış bir arşive aittir veya giriş verileri aranamaz bir arşiv akışından açılamaz. |
| ObjectDisposedException | Kaynak akış iptal edildi. |
| IOException | Bir G/Ç hatası oluştu. |

## Açıklamalar

Orijinal giriş içeriğini elde etmek için döndürülen akışı okuyun. Arşiv sağlama alanları içeriyorsa, okuma sırasında sağlama toplamı doğrulanır.

### Ayrıca Bakınız

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


