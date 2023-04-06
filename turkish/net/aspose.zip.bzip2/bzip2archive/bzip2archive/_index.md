---
title: Bzip2Archive.Bzip2Archive
second_title: Aspose.ZIP for .NET API Referansı
description: Bzip2Archive inşaatçı. Yeni bir örneğini başlatır.Bzip2Archive sıkıştırmak için hazırlanan sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

Yeni bir örneğini başlatır.[`Bzip2Archive`](../) sıkıştırmak için hazırlanan sınıf.

```csharp
public Bzip2Archive()
```

### Örnekler

Aşağıdaki örnek, bir dosyanın nasıl sıkıştırılacağını gösterir.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Ayrıca bakınız

* class [Bzip2Archive](../)
* ad alanı [Aspose.Zip.Bzip2](../../bzip2archive/)
* toplantı [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

Yeni bir örneğini başlatır.[`Bzip2Archive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public Bzip2Archive(Stream sourceStream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceStream | Stream | Arşivin kaynağı. |

### Notlar

Bu yapıcı sıkıştırmayı açmaz. Görmek[`Open`](../open/) açma yöntemi.

### Örnekler

Bir akıştan bir arşiv açın ve onu bir klasöre çıkartın.`Bellek Akışı`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### Ayrıca bakınız

* class [Bzip2Archive](../)
* ad alanı [Aspose.Zip.Bzip2](../../bzip2archive/)
* toplantı [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

Yeni bir örneğini başlatır.[`Bzip2Archive`](../) sıkıştırmayı açmak için hazırlanan sınıf.

```csharp
public Bzip2Archive(string path)
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

Bu yapıcı sıkıştırmayı açmaz. Görmek[`Open`](../open/) açma yöntemi.

### Örnekler

Dosyadan yola göre bir arşiv açın ve onu bir klasöre çıkartın.`Bellek Akışı`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### Ayrıca bakınız

* class [Bzip2Archive](../)
* ad alanı [Aspose.Zip.Bzip2](../../bzip2archive/)
* toplantı [Aspose.Zip](../../../)


