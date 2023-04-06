---
title: CpioArchive.CpioArchive
second_title: Aspose.ZIP for .NET API Referansı
description: CpioArchive inşaatçı. Yeni bir örneğini başlatır.CpioArchive sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

Yeni bir örneğini başlatır.[`CpioArchive`](../) sınıf.

```csharp
public CpioArchive()
```

### Örnekler

Aşağıdaki örnek, bir dosyanın nasıl sıkıştırılacağını gösterir.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Ayrıca bakınız

* class [CpioArchive](../)
* ad alanı [Aspose.Zip.Cpio](../../cpioarchive/)
* toplantı [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

Yeni bir örneğini başlatır.[`CpioArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public CpioArchive(Stream sourceStream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceStream | Stream | Arşivin kaynağı. Aranabilir olmalıdır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *sourceStream* boş. |
| ArgumentException | *sourceStream* aranmaz. |
| InvalidDataException | *sourceStream* geçerli bir cpio arşivi değil. |

### Notlar

Bu yapıcı herhangi bir girdiyi paketten çıkarmaz. Görmek[`Open`](../../cpioentry/open/)paketten çıkarma yöntemi.

### Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ayrıca bakınız

* class [CpioArchive](../)
* ad alanı [Aspose.Zip.Cpio](../../cpioarchive/)
* toplantı [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

Yeni bir örneğini başlatır.[`CpioArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public CpioArchive(string path)
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

Bu yapıcı herhangi bir girdiyi paketten çıkarmaz. Görmek[`Open`](../../cpioentry/open/)paketten çıkarma yöntemi.

### Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ayrıca bakınız

* class [CpioArchive](../)
* ad alanı [Aspose.Zip.Cpio](../../cpioarchive/)
* toplantı [Aspose.Zip](../../../)


