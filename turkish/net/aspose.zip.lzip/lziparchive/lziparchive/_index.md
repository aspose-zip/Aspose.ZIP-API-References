---
title: LzipArchive.LzipArchive
second_title: Aspose.ZIP for .NET API Referansı
description: LzipArchive inşaatçı. Yeni bir örneğini başlatır.LzipArchive .
type: docs
weight: 10
url: /tr/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

Yeni bir örneğini başlatır.[`LzipArchive`](../) .

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| settings | LzipArchiveSettings | Sözlük boyutunun tanımıyla belirli bir lzip arşivinin ayarlanması. |

### Ayrıca bakınız

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* ad alanı [Aspose.Zip.Lzip](../../lziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## LzipArchive(Stream) {#constructor_1}

Yeni bir örneğini başlatır.[`LzipArchive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public LzipArchive(Stream sourceStream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceStream | Stream | Arşivin kaynağı. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | *sourceStream* aranmaz. |
| ArgumentNullException | *sourceStream* boş. |
| InvalidDataException | Başlıklar, lzip tipi arşivle eşleşmiyor. |

### Notlar

Bu yapıcı sıkıştırmayı açmaz. Görmek[`Extract`](../extract/) açma yöntemi.

### Ayrıca bakınız

* class [LzipArchive](../)
* ad alanı [Aspose.Zip.Lzip](../../lziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## LzipArchive(string) {#constructor_2}

Yeni bir örneğini başlatır.[`LzipArchive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public LzipArchive(string path)
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
| InvalidDataException | Başlıklar, lzip tipi arşivle eşleşmiyor. |

### Notlar

Bu yapıcı sıkıştırmayı açmaz. Görmek[`Extract`](../extract/) açma yöntemi.

### Örnekler

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### Ayrıca bakınız

* class [LzipArchive](../)
* ad alanı [Aspose.Zip.Lzip](../../lziparchive/)
* toplantı [Aspose.Zip](../../../)


