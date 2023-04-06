---
title: SevenZipArchive.Save
second_title: Aspose.ZIP for .NET API Referansı
description: SevenZipArchive yöntem. 7z arşivini sağlanan akışa kaydeder.
type: docs
weight: 80
url: /tr/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

7z arşivini sağlanan akışa kaydeder.

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
| InvalidOperationException | Kodlayıcı verileri sıkıştıramadı. |

### Notlar

*output* aranabilir olmalıdır.

### Örnekler

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### Ayrıca bakınız

* class [SevenZipArchive](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Arşivi sağlanan hedef dosyaya kaydeder.

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

### Notlar

Bir arşivi,. adresinden yüklendiği yola kaydetmek mümkündür. Ancak, bu yaklaşım geçici dosyaya kopyalamayı kullandığından bu önerilmez.

### Örnekler

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### Ayrıca bakınız

* class [SevenZipArchive](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchive/)
* toplantı [Aspose.Zip](../../../)


