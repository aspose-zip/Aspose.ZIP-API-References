---
title: Archive.SaveSplit
second_title: Aspose.ZIP for .NET API Referansı
description: Archive yöntem. Çok ciltli arşivi sağlanan hedef dizine kaydeder.
type: docs
weight: 100
url: /tr/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

Çok ciltli arşivi sağlanan hedef dizine kaydeder.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destinationDirectory | String | Arşiv bölümlerinin oluşturulacağı dizinin yolu. |
| options | SplitArchiveSaveOptions | Dosya adı da dahil olmak üzere arşiv kaydetme seçenekleri. |

### istisnalar

| istisna | şart |
| --- | --- |
| InvalidOperationException | Bu arşiv mevcut kaynaktan açıldı. |
| NotSupportedException | Bu arşiv hem XZ yöntemiyle sıkıştırılmış hem de şifrelenmiştir. |
| ArgumentNullException | *destinationDirectory* boş. |
| SecurityException | Arayan, dizine erişmek için gerekli izne sahip değil. |
| ArgumentException | *destinationDirectory* ", &gt;, &lt; veya &#x7C; gibi geçersiz karakterler içeriyor. |
| PathTooLongException | Belirtilen yol, sistem tarafından tanımlanan maksimum uzunluğu aşıyor. |

### Notlar

Bu yöntem birkaç tane oluşturur (`N`) dosyalar dosyaadı.z01, dosyaadı.z02, ..., dosyaadı.z(n-1), dosyaadı.zip.

Mevcut arşiv çok ciltli yapılamaz.

### Örnekler

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Ayrıca bakınız

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* ad alanı [Aspose.Zip](../../archive/)
* toplantı [Aspose.Zip](../../../)


