---
title: GzipArchive.SetSource
second_title: Aspose.ZIP for .NET API Referansı
description: GzipArchive yöntem. Arşiv içinde sıkıştırılacak içeriği ayarlar.
type: docs
weight: 70
url: /tr/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(Stream source)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| source | Stream | Arşiv için giriş akışı. |

### Örnekler

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### Ayrıca bakınız

* class [GzipArchive](../)
* ad alanı [Aspose.Zip.Gzip](../../gziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileInfo | FileInfo | Sıkıştırılacak bir dosyaya başvuru. |

### Örnekler

Bir akıştan bir arşiv açın ve onu bir klasöre çıkartın.`Bellek Akışı`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### Ayrıca bakınız

* class [GzipArchive](../)
* ad alanı [Aspose.Zip.Gzip](../../gziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(string path)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Sıkıştırılacak dosyanın yolu. |

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

Dosyadan yola göre bir arşiv açın ve onu bir klasöre çıkartın.`Bellek Akışı`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Ayrıca bakınız

* class [GzipArchive](../)
* ad alanı [Aspose.Zip.Gzip](../../gziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## SetSource(TarArchive) {#setsource}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(TarArchive tarArchive)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| tarArchive | TarArchive | Tar arşivi sıkıştırılacak. |

### Notlar

Ortak tar.gz arşivi oluşturmak için bu yöntemi kullanın.

### Örnekler

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var gzippedArchive = new GzipArchive())
    {
           gzippedArchive.SetSource(tarArchive);
           gzippedArchive.Save("archive.tar.gz");
    }
}
```

### Ayrıca bakınız

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* ad alanı [Aspose.Zip.Gzip](../../gziparchive/)
* toplantı [Aspose.Zip](../../../)


