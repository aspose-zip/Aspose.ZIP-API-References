---
title: CabEntry.Extract
second_title: Aspose.ZIP for .NET API Referansı
description: CabEntry yöntem. Girdiyi sağlanan yolla dosya sistemine çıkarır.
type: docs
weight: 30
url: /tr/net/aspose.zip.cab/cabentry/extract/
---
## Extract(string) {#extract}

Girdiyi sağlanan yolla dosya sistemine çıkarır.

```csharp
public FileInfo Extract(string path)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Hedef dosyanın yolu. Dosya zaten varsa, üzerine yazılacaktır. |

### Geri dönüş değeri

Oluşturulan dosyanın dosya bilgisi.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *path* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil. |
| ArgumentException | bu*path* boş, yalnızca beyaz boşluklar içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | dosyaya erişim*path* engellendi. |
| PathTooLongException | Belirtilen*path*, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | dosya*path* dizenin ortasında iki nokta üst üste (:) içerir. |

### Örnekler

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Ayrıca bakınız

* class [CabEntry](../)
* ad alanı [Aspose.Zip.Cab](../../cabentry/)
* toplantı [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Girdiyi sağlanan akışa çıkarır.

```csharp
public void Extract(Stream destination)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destination | Stream | Hedef akışı. Yazılabilir olmalıdır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | *destination* yazmayı desteklemez. |

### Örnekler

Kabin arşivinin bir girişini çıkarın.

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Ayrıca bakınız

* class [CabEntry](../)
* ad alanı [Aspose.Zip.Cab](../../cabentry/)
* toplantı [Aspose.Zip](../../../)


