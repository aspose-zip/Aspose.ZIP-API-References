---
title: SnappyArchive.Extract
second_title: Aspose.ZIP for .NET API Referansı
description: SnappyArchive yöntem. Hızlı arşivi bir akışa çıkarır.
type: docs
weight: 30
url: /tr/net/aspose.zip.snappy/snappyarchive/extract/
---
## Extract(Stream) {#extract_2}

Hızlı arşivi bir akışa çıkarır.

```csharp
public void Extract(Stream destination)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destination | Stream | Sıkıştırılmış verileri depolamak için akış. |

### istisnalar

| istisna | şart |
| --- | --- |
| InvalidOperationException | Arşiv başlıkları ve hizmet bilgileri okunmadı. |
| InvalidDataException | Başlık veya sağlama toplamındaki verilerde hata. |
| ArgumentNullException | Hedef akış boş. |
| ArgumentException | Hedef akış yazmayı desteklemiyor. |

### Örnekler

```csharp
using (FileStream sourceSnappyFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
   {
       using (var archive = new SnappyArchive(sourceSnappyFile))
       {
           archive.Extract(extractedFile);
       }
   }
}
```

### Ayrıca bakınız

* class [SnappyArchive](../)
* ad alanı [Aspose.Zip.Snappy](../../snappyarchive/)
* toplantı [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Hızlı arşivi bir dosyaya çıkarır.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileInfo | FileInfo | Sıkıştırılmış verileri depolamak için FileInfo. |

### istisnalar

| istisna | şart |
| --- | --- |
| InvalidOperationException | Arşiv başlıkları ve hizmet bilgileri okunmadı. |
| SecurityException | Arayan, açmak için gerekli izne sahip değil.*fileInfo*. |
| ArgumentException | Dosya yolu boş veya yalnızca beyaz boşluklar içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| UnauthorizedAccessException | Dosya yolu salt okunurdur veya bir dizindir. |
| ArgumentNullException | *fileInfo* boş. |
| DirectoryNotFoundException | Eşlenmemiş bir sürücüde olmak gibi, belirtilen yol geçersiz. |
| IOException | Dosya zaten açık. |

### Örnekler

```csharp
using (FileStream snappyFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new SnappyArchive(snappyFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Ayrıca bakınız

* class [SnappyArchive](../)
* ad alanı [Aspose.Zip.Snappy](../../snappyarchive/)
* toplantı [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Hızlı arşivi yola göre bir dosyaya çıkarır.

```csharp
public FileInfo Extract(string path)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Sıkıştırılmış verileri depolayacak dosyanın yolu. |

### istisnalar

| istisna | şart |
| --- | --- |
| InvalidOperationException | Arşiv başlıkları ve hizmet bilgileri okunmadı. |
| ArgumentNullException | *path* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil. |
| ArgumentException | bu*path* boş, yalnızca beyaz boşluklar içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | dosyaya erişim*path* engellendi. |
| PathTooLongException | Belirtilen*path*, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | dosya*path* dizenin ortasında iki nokta üst üste (:) içerir. |

### Örnekler

```csharp
using (FileStream snappyFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new SnappyArchive(snappyFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Ayrıca bakınız

* class [SnappyArchive](../)
* ad alanı [Aspose.Zip.Snappy](../../snappyarchive/)
* toplantı [Aspose.Zip](../../../)


