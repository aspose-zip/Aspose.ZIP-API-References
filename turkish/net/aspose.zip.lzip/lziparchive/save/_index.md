---
title: LzipArchive.Save
second_title: Aspose.ZIP for .NET API Referansı
description: LzipArchive yöntem. lzip arşivini sağlanan akışa kaydeder.
type: docs
weight: 50
url: /tr/net/aspose.zip.lzip/lziparchive/save/
---
## Save(Stream) {#save_1}

lzip arşivini sağlanan akışa kaydeder.

```csharp
public void Save(Stream outputStream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| outputStream | Stream | Hedef akışı. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | *outputStream* aramayı desteklemez. |
| ArgumentNullException | *outputStream* boş. |

### Notlar

*outputStream* aranabilir olmalıdır.

### Örnekler

```csharp
using (FileStream lzFile = File.Open("archive.lz", FileMode.Create))
{
    using (var archive = new LzipArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzFile);
     }
}
```

### Ayrıca bakınız

* class [LzipArchive](../)
* ad alanı [Aspose.Zip.Lzip](../../lziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

lzip arşivini sağlanan hedef dosyaya kaydeder.

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
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lz");
}
```

### Ayrıca bakınız

* class [LzipArchive](../)
* ad alanı [Aspose.Zip.Lzip](../../lziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

lzip arşivini sağlanan hedef dosyaya kaydeder.

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
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz"));
}
```

### Ayrıca bakınız

* class [LzipArchive](../)
* ad alanı [Aspose.Zip.Lzip](../../lziparchive/)
* toplantı [Aspose.Zip](../../../)


