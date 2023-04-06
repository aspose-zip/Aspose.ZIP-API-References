---
title: SevenZipArchive.SaveSplit
second_title: Aspose.ZIP for .NET API Referansı
description: SevenZipArchive yöntem. Çok ciltli arşivi sağlanan hedef dizine kaydeder.
type: docs
weight: 90
url: /tr/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Çok ciltli arşivi sağlanan hedef dizine kaydeder.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destinationDirectory | String | Arşiv bölümlerinin oluşturulacağı dizinin yolu. |
| options | SplitSevenZipArchiveSaveOptions | Dosya adı da dahil olmak üzere arşiv kaydetme seçenekleri. |

### istisnalar

| istisna | şart |
| --- | --- |
| InvalidOperationException | Bu arşiv mevcut kaynaktan açıldı. |
| ArgumentNullException | *destinationDirectory* boş. |
| SecurityException | Arayan, dizine erişmek için gerekli izne sahip değil. |
| ArgumentException | *destinationDirectory* ", &gt;, &lt; veya &#x7C; gibi geçersiz karakterler içeriyor. |
| PathTooLongException | Belirtilen yol, sistem tarafından tanımlanan maksimum uzunluğu aşıyor. |

### Notlar

Bu yöntem birkaç tane oluşturur (`N`) dosyalar dosyaadı.7z.001, dosyaadı.7z.002, ..., dosyaadı.7z.(n).

Mevcut arşiv çok ciltli yapılamaz.

### Örnekler

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### Ayrıca bakınız

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchive/)
* toplantı [Aspose.Zip](../../../)


