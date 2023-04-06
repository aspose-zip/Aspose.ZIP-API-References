---
title: LzmaArchive.LzmaArchive
second_title: Aspose.ZIP for .NET API Referansı
description: LzmaArchive inşaatçı. Yeni bir örneğini başlatır.LzmaArchive sınıfını oluşturur ve arşivi lzma biçiminde oluşturur.
type: docs
weight: 10
url: /tr/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

Yeni bir örneğini başlatır.[`LzmaArchive`](../) sınıfını oluşturur ve arşivi lzma biçiminde oluşturur.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| settings | LzmaArchiveSettings | Belirli lzma arşivini ayarlama seti. |

### Ayrıca bakınız

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* ad alanı [Aspose.Zip.LZMA](../../lzmaarchive/)
* toplantı [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

Yeni bir örneğini başlatır.[`LzmaArchive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public LzmaArchive(Stream source)
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

* class [LzmaArchive](../)
* ad alanı [Aspose.Zip.LZMA](../../lzmaarchive/)
* toplantı [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

Yeni bir örneğini başlatır.[`LzmaArchive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public LzmaArchive(string path)
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

### Örnekler

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Ayrıca bakınız

* class [LzmaArchive](../)
* ad alanı [Aspose.Zip.LZMA](../../lzmaarchive/)
* toplantı [Aspose.Zip](../../../)


