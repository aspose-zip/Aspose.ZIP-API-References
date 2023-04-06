---
title: Archive.CreateEntries
second_title: Aspose.ZIP for .NET API Referansı
description: Archive yöntem. Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler.
type: docs
weight: 40
url: /tr/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| directory | DirectoryInfo | Sıkıştırılacak dizin. |
| includeRootDirectory | Boolean | Kök dizinin kendisinin dahil edilip edilmeyeceğini belirtir. |

### Geri dönüş değeri

Oluşturulan girişleri içeren arşiv.

### istisnalar

| istisna | şart |
| --- | --- |
| DirectoryNotFoundException | yolu*directory* eşlenmemiş bir sürücüde olmak gibi geçersizdir. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil*directory*. |

### Örnekler

```csharp
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### Ayrıca bakınız

* class [Archive](../)
* ad alanı [Aspose.Zip](../../archive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceDirectory | String | Sıkıştırılacak dizin. |
| includeRootDirectory | Boolean | Kök dizinin kendisinin dahil edilip edilmeyeceğini belirtir. |

### Geri dönüş değeri

Oluşturulan girişleri içeren arşiv.

### Örnekler

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### Ayrıca bakınız

* class [Archive](../)
* ad alanı [Aspose.Zip](../../archive/)
* toplantı [Aspose.Zip](../../../)


