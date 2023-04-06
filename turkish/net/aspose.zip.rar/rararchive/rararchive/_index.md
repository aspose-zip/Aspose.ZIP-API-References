---
title: RarArchive.RarArchive
second_title: Aspose.ZIP for .NET API Referansı
description: RarArchive inşaatçı. Yeni bir örneğini başlatır.RarArchive class ve composes girişleri listesi arşivden çıkarılabilir.
type: docs
weight: 10
url: /tr/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

Yeni bir örneğini başlatır.[`RarArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Arşiv dosyasının tam veya göreli yolu. |
| loadOptions | RarArchiveLoadOptions | Mevcut arşivi yüklemek için seçenekler. |

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

Bu yapıcı herhangi bir girdiyi açmaz. Görmek[`Open`](../../rararchiveentry/open/) açma yöntemi.

### Örnekler

Aşağıdaki örnek, bir arşivi ayıklayın, ardından ilk girdiyi sıkıştırılmış bir dosyaya açın.`Bellek Akışı`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Ayrıca bakınız

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* ad alanı [Aspose.Zip.Rar](../../rararchive/)
* toplantı [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

Yeni bir örneğini başlatır.[`RarArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceStream | Stream | Arşivin kaynağı. |
| loadOptions | RarArchiveLoadOptions | Mevcut arşivi yüklemek için seçenekler. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | *sourceStream* aranmaz. |
| InvalidDataException | Arşiv için yanlış imza. - veya - Dosya bir RAR arşivi değil. |
| InvalidOperationException |  |

### Notlar

Bu yapıcı herhangi bir girdiyi açmaz. Görmek[`Open`](../../rararchiveentry/open/) açma yöntemi.

### Örnekler

Aşağıdaki örnek, bir dosyaya ilk girişi deşifre eder ve açar.`Bellek Akışı`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Ayrıca bakınız

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* ad alanı [Aspose.Zip.Rar](../../rararchive/)
* toplantı [Aspose.Zip](../../../)


