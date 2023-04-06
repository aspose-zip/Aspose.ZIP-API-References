---
title: XzArchive.Save
second_title: Aspose.ZIP for .NET API Referansı
description: XzArchive yöntem. xz arşivini sağlanan akışa kaydeder.
type: docs
weight: 40
url: /tr/net/aspose.zip.xz/xzarchive/save/
---
## Save(Stream) {#save}

xz arşivini sağlanan akışa kaydeder.

```csharp
public void Save(Stream output)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| output | Stream | Hedef akışı. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | *output* aramayı desteklemez. |
| ArgumentNullException | *output* boş. |

### Notlar

*output* aranabilir olmalıdır.

### Örnekler

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    using (var archive = new XzArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Ayrıca bakınız

* class [XzArchive](../)
* ad alanı [Aspose.Zip.Xz](../../xzarchive/)
* toplantı [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

xz arşivini sağlanan hedef dosyaya kaydeder.

```csharp
public void Save(string destinationFileName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destinationFileName | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *destinationFileName* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil. |
| ArgumentException | bu*destinationFileName* boş, yalnızca beyaz boşluklar içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | dosyaya erişim*destinationFileName* engellendi. |
| PathTooLongException | Belirtilen*destinationFileName*, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | dosya*destinationFileName* dizenin ortasında iki nokta üst üste (:) içerir. |

### Örnekler

```csharp
using (var archive = new XzArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.xz");
}
```

### Ayrıca bakınız

* class [XzArchive](../)
* ad alanı [Aspose.Zip.Xz](../../xzarchive/)
* toplantı [Aspose.Zip](../../../)


