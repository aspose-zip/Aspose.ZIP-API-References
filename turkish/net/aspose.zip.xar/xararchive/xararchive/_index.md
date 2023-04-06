---
title: XarArchive.XarArchive
second_title: Aspose.ZIP for .NET API Referansı
description: XarArchive inşaatçı. Yeni bir örneğini başlatır.XarArchive class ve composes girişleri listesi arşivden çıkarılabilir.
type: docs
weight: 10
url: /tr/net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(Stream) {#constructor}

Yeni bir örneğini başlatır.[`XarArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public XarArchive(Stream sourceStream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceStream | Stream | Arşivin kaynağı. Aranabilir olmalıdır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *sourceStream* boş. |
| ArgumentException | *sourceStream* aranmaz. |
| InvalidDataException | *sourceStream* geçerli bir xar arşivi değil. |

### Notlar

Bu yapıcı herhangi bir girdiyi paketten çıkarmaz. Görmek[`Open`](../../xarfileentry/open/)paketten çıkarma yöntemi.

### Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Ayrıca bakınız

* class [XarArchive](../)
* ad alanı [Aspose.Zip.Xar](../../xararchive/)
* toplantı [Aspose.Zip](../../../)

---

## XarArchive(string) {#constructor_1}

Yeni bir örneğini başlatır.[`XarArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public XarArchive(string path)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Arşiv dosyasının yolu. |

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

Bu yapıcı herhangi bir girdiyi paketten çıkarmaz. Görmek[`Open`](../../xarfileentry/open/)paketten çıkarma yöntemi.

### Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Ayrıca bakınız

* class [XarArchive](../)
* ad alanı [Aspose.Zip.Xar](../../xararchive/)
* toplantı [Aspose.Zip](../../../)


