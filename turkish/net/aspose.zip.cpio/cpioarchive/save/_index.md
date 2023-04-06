---
title: CpioArchive.Save
second_title: Aspose.ZIP for .NET API Referansı
description: CpioArchive yöntem. Arşivi sağlanan hedef dosyaya kaydeder.
type: docs
weight: 80
url: /tr/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

Arşivi sağlanan hedef dosyaya kaydeder.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destinationFileName | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| cpioFormat | CpioFormat | cpio başlık biçimini tanımlar. |

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
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### Ayrıca bakınız

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* ad alanı [Aspose.Zip.Cpio](../../cpioarchive/)
* toplantı [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

Arşivi sağlanan akışa kaydeder.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| output | Stream | Hedef akışı. |
| cpioFormat | CpioFormat | cpio başlık biçimini tanımlar. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *output* boş. |
| ArgumentException | *output* yazılabilir değil. - veya -*output* çıkardığımız akışın aynısıdır. - VEYA - Arşivi şuraya kaydetmek imkansızdır:*cpioFormat* biçim kısıtlamaları nedeniyle. |

### Notlar

*output*yazılabilir olmalıdır.

### Örnekler

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(cpioFile);
    }
}       
```

### Ayrıca bakınız

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* ad alanı [Aspose.Zip.Cpio](../../cpioarchive/)
* toplantı [Aspose.Zip](../../../)


