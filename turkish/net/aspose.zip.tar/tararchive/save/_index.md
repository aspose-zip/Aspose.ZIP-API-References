---
title: TarArchive.Save
second_title: Aspose.ZIP for .NET API Referansı
description: TarArchive yöntem. Arşivi sağlanan akışa kaydeder.
type: docs
weight: 120
url: /tr/net/aspose.zip.tar/tararchive/save/
---
## Save(Stream, TarFormat?) {#save}

Arşivi sağlanan akışa kaydeder.

```csharp
public void Save(Stream output, TarFormat? format = default)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| output | Stream | Hedef akışı. |
| format | Nullable`1 | tar başlık biçimini tanımlar. Boş değer, mümkün olduğunda USar olarak ele alınacaktır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | *output* yazılabilir değil. - veya -*output* çıkardığımız akışın aynısıdır. - VEYA - Arşivi şuraya kaydetmek imkansızdır:*format* biçim kısıtlamaları nedeniyle. |

### Notlar

*output*yazılabilir olmalıdır.

### Örnekler

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(tarFile);
    }
}       
```

### Ayrıca bakınız

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)

---

## Save(string, TarFormat?) {#save_1}

Arşivi sağlanan hedef dosyaya kaydeder.

```csharp
public void Save(string destinationFileName, TarFormat? format = default)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destinationFileName | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| format | Nullable`1 | tar başlık biçimini tanımlar. Boş değer, mümkün olduğunda USar olarak ele alınacaktır. |

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
using (var archive = new TarArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("myarchive.tar");
}       
```

### Ayrıca bakınız

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)


