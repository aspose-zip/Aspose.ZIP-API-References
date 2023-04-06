---
title: SnappyArchive.SnappyArchive
second_title: Aspose.ZIP for .NET API Referansı
description: SnappyArchive inşaatçı. Yeni bir örneğini başlatır.SnappyArchive sıkıştırmak için hazırlanan sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

Yeni bir örneğini başlatır.[`SnappyArchive`](../) sıkıştırmak için hazırlanan sınıf.

```csharp
public SnappyArchive()
```

### Örnekler

Aşağıdaki örnek, bir dosyanın nasıl sıkıştırılacağını gösterir.

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snapy");
}
```

### Ayrıca bakınız

* class [SnappyArchive](../)
* ad alanı [Aspose.Zip.Snappy](../../snappyarchive/)
* toplantı [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

Yeni bir örneğini başlatır.[`SnappyArchive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public SnappyArchive(Stream source)
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

* class [SnappyArchive](../)
* ad alanı [Aspose.Zip.Snappy](../../snappyarchive/)
* toplantı [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

Yeni bir örneğini başlatır.[`SnappyArchive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public SnappyArchive(string path)
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
    using (var archive = new SnappyArchive(sourceSnappyFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Ayrıca bakınız

* class [SnappyArchive](../)
* ad alanı [Aspose.Zip.Snappy](../../snappyarchive/)
* toplantı [Aspose.Zip](../../../)


