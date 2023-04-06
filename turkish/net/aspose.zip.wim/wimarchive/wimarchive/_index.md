---
title: WimArchive.WimArchive
second_title: Aspose.ZIP for .NET API Referansı
description: WimArchive inşaatçı. Yeni bir örneğini başlatır.WimArchive class ve composes girişleri listesi arşivden çıkarılabilir.
type: docs
weight: 10
url: /tr/net/aspose.zip.wim/wimarchive/wimarchive/
---
## WimArchive(Stream) {#constructor}

Yeni bir örneğini başlatır.[`WimArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public WimArchive(Stream sourceStream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceStream | Stream | Arşivin kaynağı. Aranabilir olmalıdır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *sourceStream* boş. |
| ArgumentException | *sourceStream* aranmaz. |
| InvalidDataException | *sourceStream* geçerli wim arşivi değil. |

### Notlar

Bu yapıcı herhangi bir girdiyi paketten çıkarmaz. Görmek[`Open`](../../wimfileentry/open/)paketten çıkarma yöntemi.

### Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new WimArchive(File.OpenRead("archive.wim")))
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### Ayrıca bakınız

* class [WimArchive](../)
* ad alanı [Aspose.Zip.Wim](../../wimarchive/)
* toplantı [Aspose.Zip](../../../)

---

## WimArchive(string) {#constructor_1}

Yeni bir örneğini başlatır.[`WimArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public WimArchive(string path)
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

Bu yapıcı herhangi bir girdiyi paketten çıkarmaz. Görmek[`Open`](../../wimfileentry/open/)paketten çıkarma yöntemi.

### Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### Ayrıca bakınız

* class [WimArchive](../)
* ad alanı [Aspose.Zip.Wim](../../wimarchive/)
* toplantı [Aspose.Zip](../../../)


