---
title: XzArchive.XzArchive
second_title: Aspose.ZIP for .NET API Referansı
description: XzArchive inşaatçı. Yeni bir örneğini başlatır.XzArchive sınıfını oluşturur ve arşivi xz formatında oluşturur.
type: docs
weight: 10
url: /tr/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Yeni bir örneğini başlatır.[`XzArchive`](../) sınıfını oluşturur ve arşivi xz formatında oluşturur.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| settings | XzArchiveSettings | Belirli xz arşivi ayar kümesi: sözlük boyutu, blok boyutu, kontrol tipi. |

### Ayrıca bakınız

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* ad alanı [Aspose.Zip.Xz](../../xzarchive/)
* toplantı [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

Yeni bir örneğini başlatır.[`XzArchive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public XzArchive(Stream source)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| source | Stream | Arşivin kaynağı. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | *source* aranmaz. |
| ArgumentNullException | *source* boş. |

### Notlar

Bu yapıcı sıkıştırmayı açmaz. Görmek[`Extract`](../extract/) açma yöntemi.

### Ayrıca bakınız

* class [XzArchive](../)
* ad alanı [Aspose.Zip.Xz](../../xzarchive/)
* toplantı [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

Yeni bir örneğini başlatır.[`XzArchive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public XzArchive(string path)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Arşiv kaynağına giden yol. |

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

Bu yapıcı sıkıştırmayı açmaz. Görmek[`Extract`](../extract/) açma yöntemi.

### Ayrıca bakınız

* class [XzArchive](../)
* ad alanı [Aspose.Zip.Xz](../../xzarchive/)
* toplantı [Aspose.Zip](../../../)


