---
title: TarArchive.FromGZip
second_title: Aspose.ZIP for .NET API Referansı
description: TarArchive yöntem. Sağlanan gzip arşivini çıkarır ve oluştururTarArchive çıkarılan verilerden.
type: docs
weight: 20
url: /tr/net/aspose.zip.tar/tararchive/fromgzip/
---
## FromGZip(Stream) {#fromgzip}

Sağlanan gzip arşivini çıkarır ve oluşturur[`TarArchive`](../) çıkarılan verilerden.

Önemli: gzip arşivi bu metot içerisinde tamamen çıkartılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

```csharp
public static TarArchive FromGZip(Stream source)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| source | Stream | Arşivin kaynağı. |

### Geri dönüş değeri

bir örneği[`TarArchive`](../)

### Notlar

GZip çıkarma akışı, sıkıştırma algoritmasının doğası gereği aranamaz. Tar arşivi, rastgele kayıt çıkarma olanağı sağlar, bu nedenle, başlık altında aranabilir akışı çalıştırması gerekir.

### Ayrıca bakınız

* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)

---

## FromGZip(string) {#fromgzip_1}

Sağlanan gzip arşivini çıkarır ve oluşturur[`TarArchive`](../) çıkarılan verilerden.

Önemli: gzip arşivi bu metot içerisinde tamamen çıkartılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

```csharp
public static TarArchive FromGZip(string path)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Arşiv dosyasının yolu. |

### Geri dönüş değeri

bir örneği[`TarArchive`](../)

### Notlar

GZip çıkarma akışı, sıkıştırma algoritmasının doğası gereği aranamaz. Tar arşivi, rastgele kayıt çıkarma olanağı sağlar, bu nedenle, başlık altında aranabilir akışı çalıştırması gerekir.

### Ayrıca bakınız

* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)


