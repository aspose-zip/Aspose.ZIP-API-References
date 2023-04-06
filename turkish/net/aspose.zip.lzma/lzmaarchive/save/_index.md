---
title: LzmaArchive.Save
second_title: Aspose.ZIP for .NET API Referansı
description: LzmaArchive yöntem. lzma arşivini sağlanan akışa kaydeder.
type: docs
weight: 40
url: /tr/net/aspose.zip.lzma/lzmaarchive/save/
---
## Save(Stream) {#save_1}

lzma arşivini sağlanan akışa kaydeder.

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

### Notlar

*output* aranabilir olmalıdır.

### Örnekler

```csharp
using (FileStream lzmaFile = File.Open("archive.lzma", FileMode.Create))
{
    using (var archive = new LzmaArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzmaFile);
     }
}
```

### Ayrıca bakınız

* class [LzmaArchive](../)
* ad alanı [Aspose.Zip.LZMA](../../lzmaarchive/)
* toplantı [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

lzma arşivini sağlanan hedef dosyaya kaydeder.

```csharp
public void Save(FileInfo destination)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destination | FileInfo | Hedef akış olarak açılacak olan FileInfo. |

### istisnalar

| istisna | şart |
| --- | --- |
| SecurityException | Arayan, açmak için gerekli izne sahip değil.*destination*. |
| ArgumentException | Dosya yolu boş veya yalnızca beyaz boşluklar içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| UnauthorizedAccessException | Dosya yolu salt okunurdur veya bir dizindir. |
| ArgumentNullException | *destination* boş. |
| DirectoryNotFoundException | Eşlenmemiş bir sürücüde olmak gibi, belirtilen yol geçersiz. |
| IOException | Dosya zaten açık. |

### Örnekler

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lzma"));
}
```

### Ayrıca bakınız

* class [LzmaArchive](../)
* ad alanı [Aspose.Zip.LZMA](../../lzmaarchive/)
* toplantı [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

lzma arşivini sağlanan hedef dosyaya kaydeder.

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

### Örnekler

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lzma");
}
```

### Ayrıca bakınız

* class [LzmaArchive](../)
* ad alanı [Aspose.Zip.LZMA](../../lzmaarchive/)
* toplantı [Aspose.Zip](../../../)


