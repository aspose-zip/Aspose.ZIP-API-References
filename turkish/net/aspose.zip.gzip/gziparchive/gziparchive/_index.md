---
title: GzipArchive.GzipArchive
second_title: Aspose.ZIP for .NET API Referansı
description: GzipArchive inşaatçı. Yeni bir örneğini başlatır.GzipArchive sıkıştırmak için hazırlanan sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

Yeni bir örneğini başlatır.[`GzipArchive`](../) sıkıştırmak için hazırlanan sınıf.

```csharp
public GzipArchive()
```

### Örnekler

Aşağıdaki örnek, bir dosyanın nasıl sıkıştırılacağını gösterir.

```csharp
using (GzipArchive archive = new GzipArchive()) 
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

## GzipArchive(Stream, bool) {#constructor_1}

Yeni bir örneğini başlatır.[`GzipArchive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceStream | Stream | Arşivin kaynağı. |
| parseHeader | Boolean | Ad da dahil olmak üzere özellikleri bulmak için akış başlığının ayrıştırılıp ayrıştırılmayacağı. Yalnızca aranabilir akış için anlamlıdır. |

### Notlar

Bu yapıcı sıkıştırmayı açmaz. Görmek[`Open`](../open/) açma yöntemi.

### Örnekler

Bir akıştan bir arşiv açın ve onu bir klasöre çıkartın.`Bellek Akışı`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### Ayrıca bakınız

* class [GzipArchive](../)
* ad alanı [Aspose.Zip.Gzip](../../gziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

Yeni bir örneğini başlatır.[`GzipArchive`](../) sınıf.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Arşiv dosyasının yolu. |
| parseHeader | Boolean | Ad da dahil olmak üzere özellikleri bulmak için akış başlığının ayrıştırılıp ayrıştırılmayacağı. Yalnızca aranabilir akış için anlamlıdır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *path* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil. |
| ArgumentException | bu*path* boş, yalnızca beyaz boşluklar içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | dosyaya erişim*path* engellendi. |
| PathTooLongException | Belirtilen*path*, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | dosya*path* dizenin ortasında iki nokta üst üste (:) içerir. |

### Notlar

Bu yapıcı sıkıştırmayı açmaz. Görmek[`Open`](../open/) açma yöntemi.

### Örnekler

Dosyadan yola göre bir arşiv açın ve onu bir klasöre çıkartın.`Bellek Akışı`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### Ayrıca bakınız

* class [GzipArchive](../)
* ad alanı [Aspose.Zip.Gzip](../../gziparchive/)
* toplantı [Aspose.Zip](../../../)


