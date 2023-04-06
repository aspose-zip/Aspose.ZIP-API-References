---
title: TarArchive.TarArchive
second_title: Aspose.ZIP for .NET API Referansı
description: TarArchive inşaatçı. Yeni bir örneğini başlatır.TarArchive sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Yeni bir örneğini başlatır.[`TarArchive`](../) sınıf.

```csharp
public TarArchive()
```

### Örnekler

Aşağıdaki örnek, bir dosyanın nasıl sıkıştırılacağını gösterir.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### Ayrıca bakınız

* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

Yeni bir örneğini başlatır.[`Archive`](../../../aspose.zip/archive/) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public TarArchive(Stream sourceStream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceStream | Stream | Arşivin kaynağı. Aranabilir olmalıdır. |

### istisnalar

| istisna | şart |
| --- | --- |
| InvalidDataException | *sourceStream* aranmaz. |

### Notlar

Bu yapıcı herhangi bir girdiyi paketten çıkarmaz. Görmek[`Open`](../../tarentry/open/)paketten çıkarma yöntemi.

### Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ayrıca bakınız

* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

Yeni bir örneğini başlatır.[`TarArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public TarArchive(string path)
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

Bu yapıcı herhangi bir girdiyi paketten çıkarmaz. Görmek[`Open`](../../tarentry/open/)paketten çıkarma yöntemi.

### Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ayrıca bakınız

* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)


