---
title: ArchiveEntry.Extract
second_title: Aspose.ZIP for .NET API Referansı
description: ArchiveEntry yöntem. Girdiyi sağlanan yolla dosya sistemine çıkarır.
type: docs
weight: 100
url: /tr/net/aspose.zip/archiveentry/extract/
---
## Extract(string, string) {#extract}

Girdiyi sağlanan yolla dosya sistemine çıkarır.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Hedef dosyanın yolu. Dosya zaten varsa, üzerine yazılacaktır. |
| password | String | Şifre çözme için isteğe bağlı şifre. |

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
| InvalidDataException | Giriş için CRC veya MAC doğrulaması başarısız oldu. |

### Örnekler

Her biri kendi şifresine sahip iki zip arşivi girişini çıkarın

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract("first.bin", "first_pass");
        archive.Entries[1].Extract("second.bin", "second_pass");
    }
}
```

### Ayrıca bakınız

* class [ArchiveEntry](../)
* ad alanı [Aspose.Zip](../../archiveentry/)
* toplantı [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Girdiyi sağlanan akışa çıkarır.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destination | Stream | Hedef akışı. Yazılabilir olmalıdır. |
| password | String | Şifre çözme için isteğe bağlı şifre. |

### istisnalar

| istisna | şart |
| --- | --- |
| InvalidDataException | Giriş için CRC veya MAC doğrulaması başarısız oldu. |
| ArgumentException | *destination* yazmayı desteklemez. |

### Örnekler

Bir zip arşivi girişini şifre ile çıkarın.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### Ayrıca bakınız

* class [ArchiveEntry](../)
* ad alanı [Aspose.Zip](../../archiveentry/)
* toplantı [Aspose.Zip](../../../)


