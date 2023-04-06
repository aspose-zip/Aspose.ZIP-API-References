---
title: SevenZipArchive.CreateEntries
second_title: Aspose.ZIP for .NET API Referansı
description: SevenZipArchive yöntem. Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler.
type: docs
weight: 40
url: /tr/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler.

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
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
using (SevenZipArchive archive = new SevenZipArchive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.7z");
}
```

### Ayrıca bakınız

* class [SevenZipArchive](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler.

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceDirectory | String | Sıkıştırılacak dizin. |
| includeRootDirectory | Boolean | Kök dizinin kendisinin dahil edilip edilmeyeceğini belirtir. |

### Geri dönüş değeri

Oluşturulan girişleri içeren arşiv.

### Örnekler

LZMA2 sıkıştırması ile 7z arşivi oluşturun.

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### Ayrıca bakınız

* class [SevenZipArchive](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchive/)
* toplantı [Aspose.Zip](../../../)


