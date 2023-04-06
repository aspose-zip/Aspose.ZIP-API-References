---
title: ZArchive.ZArchive
second_title: Aspose.ZIP for .NET API Referansı
description: ZArchive inşaatçı. Yeni bir örneğini başlatır.ZArchive sıkıştırmak için hazırlanan sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

Yeni bir örneğini başlatır.[`ZArchive`](../) sıkıştırmak için hazırlanan sınıf.

```csharp
public ZArchive()
```

### Ayrıca bakınız

* class [ZArchive](../)
* ad alanı [Aspose.Zip.Z](../../zarchive/)
* toplantı [Aspose.Zip](../../../)

---

## ZArchive(Stream) {#constructor_1}

Yeni bir örneğini başlatır.[`ZArchive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public ZArchive(Stream source)
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

* class [ZArchive](../)
* ad alanı [Aspose.Zip.Z](../../zarchive/)
* toplantı [Aspose.Zip](../../../)

---

## ZArchive(string) {#constructor_2}

Yeni bir örneğini başlatır.[`ZArchive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public ZArchive(string path)
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

* class [ZArchive](../)
* ad alanı [Aspose.Zip.Z](../../zarchive/)
* toplantı [Aspose.Zip](../../../)


