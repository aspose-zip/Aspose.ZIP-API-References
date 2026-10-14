---
title: "IsoEntry.Extract"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "IsoEntry yöntemi. Girişi sağlanan yola göre dosya sistemine çıkarır"
type: docs
weight: 50
url: /tr/net/aspose.zip.iso/isoentry/extract/
---
## Extract(string) {#extract}

Girişi sağlanan yola göre dosya sistemine çıkarır.

```csharp
public FileInfo Extract(string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |

### Dönüş Değeri

Çıkarılan verileri içeren FileInfo örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| IOException | Dosya zaten açık. |
| InvalidOperationException | Arşiv başlıkları ve hizmet bilgileri okunmadı. |

### Ayrıca Bakınız

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
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
| NotSupportedException | Giriş bir dosyayı temsil etmiyorsa hata yükseltir. |
| ArgumentException | Sağlanan akış yazmayı desteklemiyor. |

### Ayrıca Bakınız

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)


