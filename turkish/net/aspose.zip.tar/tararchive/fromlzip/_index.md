---
title: TarArchive.FromLZip
second_title: Aspose.ZIP for .NET API Referansı
description: TarArchive yöntem. Sağlanan lzip arşivini çıkarır ve oluştururTarArchive çıkarılan verilerden.
type: docs
weight: 30
url: /tr/net/aspose.zip.tar/tararchive/fromlzip/
---
## FromLZip(Stream) {#fromlzip}

Sağlanan lzip arşivini çıkarır ve oluşturur[`TarArchive`](../) çıkarılan verilerden.

Önemli: lzip arşivi bu yöntemle tamamen çıkartılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

```csharp
public static TarArchive FromLZip(Stream source)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| source | Stream | Arşivin kaynağı. |

### Geri dönüş değeri

bir örneği[`TarArchive`](../)

### Notlar

Lzip çıkarma akışı, sıkıştırma algoritmasının doğası gereği aranamaz. Tar arşivi, isteğe bağlı kayıt çıkarma olanağı sağlar, bu nedenle, başlık altında aranabilir akışı çalıştırması gerekir.

### Ayrıca bakınız

* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)

---

## FromLZip(string) {#fromlzip_1}

Sağlanan lzip arşivini çıkarır ve oluşturur[`TarArchive`](../) çıkarılan verilerden.

Önemli: lzip arşivi bu yöntemle tamamen çıkartılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

```csharp
public static TarArchive FromLZip(string path)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Arşiv dosyasının yolu. |

### Geri dönüş değeri

bir örneği[`TarArchive`](../)

### Notlar

Lzip çıkarma akışı, sıkıştırma algoritmasının doğası gereği aranamaz. Tar arşivi, isteğe bağlı kayıt çıkarma olanağı sağlar, bu nedenle, başlık altında aranabilir akışı çalıştırması gerekir.

### Ayrıca bakınız

* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)


