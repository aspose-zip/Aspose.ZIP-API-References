---
title: SharArchive.CreateEntries
second_title: Aspose.ZIP for .NET API Referansı
description: SharArchive yöntem. Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler.
type: docs
weight: 30
url: /tr/net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler.

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceDirectory | String | Sıkıştırılacak dizin. |
| includeRootDirectory | Boolean | Kök dizinin kendisinin dahil edilip edilmeyeceğini belirtir. |

### Geri dönüş değeri

Paylaşım girişi örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *sourceDirectory* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil*sourceDirectory*. |
| ArgumentException | *sourceDirectory* ", &lt;, &gt; veya &#x7C; gibi geçersiz karakterler içeriyor. |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. Belirtilen yol, dosya adı veya her ikisi de çok uzun. |
| IOException | *sourceDirectory* bir dizin yerine bir dosya anlamına gelir. |

### Örnekler

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(sharFile);
    }
}
```

### Ayrıca bakınız

* class [SharArchive](../)
* ad alanı [Aspose.Zip.Shar](../../shararchive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler.

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| directory | DirectoryInfo | Sıkıştırılacak dizin. |
| includeRootDirectory | Boolean | Kök dizinin kendisinin dahil edilip edilmeyeceğini belirtir. |

### Geri dönüş değeri

Paylaşım girişi örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *directory* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil*directory*. |
| IOException | *directory* bir dizin yerine bir dosya anlamına gelir. |

### Örnekler

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(sharFile);
    }
}
```

### Ayrıca bakınız

* class [SharArchive](../)
* ad alanı [Aspose.Zip.Shar](../../shararchive/)
* toplantı [Aspose.Zip](../../../)


