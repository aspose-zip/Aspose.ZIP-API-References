---
title: CabArchive.CabArchive
second_title: Aspose.ZIP for .NET API Referansı
description: CabArchive inşaatçı. Yeni bir örneğini başlatır.CabArchive class ve composes girişleri listesi arşivden çıkarılabilir.
type: docs
weight: 10
url: /tr/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(Stream) {#constructor}

Yeni bir örneğini başlatır.[`CabArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public CabArchive(Stream sourceStream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceStream | Stream | Arşivin kaynağı. Aranabilir olmalıdır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *sourceStream* boş. |
| ArgumentException | *sourceStream* aranmaz. |
| InvalidDataException | *sourceStream* geçerli kabin arşivi değil. |

### Notlar

Bu yapıcı herhangi bir girdiyi paketten çıkarmaz. Görmek[`Open`](../../cabentry/open/)paketten çıkarma yöntemi.

### Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ayrıca bakınız

* class [CabArchive](../)
* ad alanı [Aspose.Zip.Cab](../../cabarchive/)
* toplantı [Aspose.Zip](../../../)

---

## CabArchive(string) {#constructor_1}

Yeni bir örneğini başlatır.[`CabArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public CabArchive(string path)
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

Bu yapıcı herhangi bir girdiyi paketten çıkarmaz. Görmek[`Open`](../../cabentry/open/)paketten çıkarma yöntemi.

### Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ayrıca bakınız

* class [CabArchive](../)
* ad alanı [Aspose.Zip.Cab](../../cabarchive/)
* toplantı [Aspose.Zip](../../../)


