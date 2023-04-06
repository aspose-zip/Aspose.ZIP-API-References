---
title: TarArchive.CreateEntries
second_title: Aspose.ZIP for .NET API Referansı
description: TarArchive yöntem. Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler.
type: docs
weight: 70
url: /tr/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler.

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| directory | DirectoryInfo | Sıkıştırılacak dizin. |
| includeRootDirectory | Boolean | Kök dizinin kendisinin dahil edilip edilmeyeceğini belirtir. |

### Geri dönüş değeri

Oluşturulan girişleri içeren arşiv.

### Örnekler

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### Ayrıca bakınız

* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler.

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceDirectory | String | Sıkıştırılacak dizin. |
| includeRootDirectory | Boolean | Kök dizinin kendisinin dahil edilip edilmeyeceğini belirtir. |

### Geri dönüş değeri

Oluşturulan girişleri içeren arşiv.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *sourceDirectory* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil*sourceDirectory*. |
| ArgumentException | *sourceDirectory* ", &lt;, &gt; veya &#x7C; gibi geçersiz karakterler içeriyor. |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. Belirtilen yol, dosya adı veya her ikisi de çok uzun. |

### Örnekler

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### Ayrıca bakınız

* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)


