---
title: ZArchive.SetSource
second_title: Aspose.ZIP for .NET API Referansı
description: ZArchive yöntem. Arşiv içinde sıkıştırılacak içeriği ayarlar.
type: docs
weight: 50
url: /tr/net/aspose.zip.z/zarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(Stream source)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| source | Stream | Arşiv için giriş akışı. |

### Örnekler

```csharp
using (var archive = new ZArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.Z");
}
```

### Ayrıca bakınız

* class [ZArchive](../)
* ad alanı [Aspose.Zip.Z](../../zarchive/)
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
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### Ayrıca bakınız

* class [ZArchive](../)
* ad alanı [Aspose.Zip.Z](../../zarchive/)
* toplantı [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(string sourcePath)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourcePath | String | Giriş akışı olarak açılacak dosyanın yolu. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *sourcePath* null veya boş dizedir. |
| SecurityException | Arayan, bir kaynağa erişmek için gereken izne sahip değil. |
| ArgumentException | bu*sourcePath* boş, yalnızca beyaz boşluklar içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | dosyaya erişim*sourcePath* engellendi. |
| PathTooLongException | Belirtilen*sourcePath*, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | dosya*sourcePath* dizenin ortasında iki nokta üst üste (:) içerir. |

### Örnekler

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("data.bin.Z");
}
```

### Ayrıca bakınız

* class [ZArchive](../)
* ad alanı [Aspose.Zip.Z](../../zarchive/)
* toplantı [Aspose.Zip](../../../)


