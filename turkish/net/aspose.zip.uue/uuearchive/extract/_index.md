---
title: "UueArchive.Extract"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "UueArchive yöntemi. Arşivi sağlanan akışa çıkarır"
type: docs
weight: 40
url: /tr/net/aspose.zip.uue/uuearchive/extract/
---
## Extract(Stream) {#extract_1}

Arşivi sağlanan akışa çıkarır.

```csharp
public void Extract(Stream destination)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | Akış | Hedef akış. Yazılabilir olmalıdır. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| ArgumentException | *destination* yazmayı desteklemiyor. |

## Örnekler

```csharp
using (var archive = new UueArchive("archive.uue"))
{
     archive.Extract(httpResponseStream);
}
```

### Ayrıca Bakınız

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Arşivi yola göre dosyaya çıkarır.

```csharp
public FileInfo Extract(string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |

### Dönüş Değeri

Çıkarılan dosyanın bilgisi.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| IOException | Dosya zaten açık. |
| InvalidDataException | Veri geçersiz veya bozuk olduğunda fırlatılır. |

### Ayrıca Bakınız

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


