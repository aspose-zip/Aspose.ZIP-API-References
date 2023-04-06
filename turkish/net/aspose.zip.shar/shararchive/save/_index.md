---
title: SharArchive.Save
second_title: Aspose.ZIP for .NET API Referansı
description: SharArchive yöntem. Arşivi sağlanan hedef dosyaya kaydeder.
type: docs
weight: 70
url: /tr/net/aspose.zip.shar/shararchive/save/
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
| ArgumentException | *destinationFileName* sıfır uzunluklu bir dizedir, yalnızca boşluk içerir veya System.IO.Path.InvalidPathChars tarafından tanımlandığı şekilde bir veya daha fazla geçersiz karakter içerir. |
| ArgumentNullException | *destinationFileName* boş. |
| PathTooLongException | Belirtilen*destinationFileName*, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| DirectoryNotFoundException | Belirtilen*destinationFileName* geçersiz (örneğin, eşlenmemiş bir sürücüde). |
| IOException | Dosya açılırken bir G/Ç hatası oluştu. |
| UnauthorizedAccessException | *destinationFileName* salt okunur bir dosya belirtildi ve erişim Read değil.-veya- yol bir dizin belirtildi.-veya- Arayan gerekli izne sahip değil. |
| NotSupportedException | *destinationFileName* geçersiz bir biçimdedir. |

### Notlar

Bir arşivi,. adresinden yüklendiği yola kaydetmek mümkündür. Ancak, bu yaklaşım geçici dosyaya kopyalamayı kullandığından bu önerilmez.

### Örnekler

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### Ayrıca bakınız

* class [SharArchive](../)
* ad alanı [Aspose.Zip.Shar](../../shararchive/)
* toplantı [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

Arşivi sağlanan akışa kaydeder.

```csharp
public void Save(Stream output)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| output | Stream | Hedef akışı. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *output* boş. |
| ArgumentException | *output* yazılabilir değil. - veya -*output* çıkardığımız akışın aynısıdır. |

### Notlar

*output*yazılabilir olmalıdır.

### Örnekler

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### Ayrıca bakınız

* class [SharArchive](../)
* ad alanı [Aspose.Zip.Shar](../../shararchive/)
* toplantı [Aspose.Zip](../../../)


