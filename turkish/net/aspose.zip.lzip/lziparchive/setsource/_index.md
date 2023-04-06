---
title: LzipArchive.SetSource
second_title: Aspose.ZIP for .NET API Referansı
description: LzipArchive yöntem. Arşiv içinde sıkıştırılacak içeriği ayarlar.
type: docs
weight: 60
url: /tr/net/aspose.zip.lzip/lziparchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(Stream source)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| source | Stream | Arşiv için giriş akışı. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | bu*source* akış aranmaz. |

### Örnekler

```csharp
using (var archive = new LzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz");

```

### Ayrıca bakınız

* class [LzipArchive](../)
* ad alanı [Aspose.Zip.Lzip](../../lziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileInfo | FileInfo | Giriş akışı olarak açılacak olan FileInfo. |

### istisnalar

| istisna | şart |
| --- | --- |
| SecurityException | Arayan, açmak için gerekli izne sahip değil.*fileInfo*. |
| ArgumentException | Dosya yolu boş veya yalnızca beyaz boşluklar içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| UnauthorizedAccessException | Dosya yolu salt okunurdur veya bir dizindir. |
| ArgumentNullException | *fileInfo* boş. |
| DirectoryNotFoundException | Eşlenmemiş bir sürücüde olmak gibi, belirtilen yol geçersiz. |
| IOException | Dosya zaten açık. |

### Örnekler

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz");
}
```

### Ayrıca bakınız

* class [LzipArchive](../)
* ad alanı [Aspose.Zip.Lzip](../../lziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(string path)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Sıkıştırılacak dosyanın yolu.. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *path* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil. |
| ArgumentException | bu*path* boş, yalnızca beyaz boşluklar içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | dosyaya erişim*path* engellendi. |
| PathTooLongException | Belirtilen*path*, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | dosya*path* dizenin ortasında iki nokta üst üste (:) içerir. |

### Örnekler

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz");
}
```

### Ayrıca bakınız

* class [LzipArchive](../)
* ad alanı [Aspose.Zip.Lzip](../../lziparchive/)
* toplantı [Aspose.Zip](../../../)


