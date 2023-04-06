---
title: SevenZipArchive.SevenZipArchive
second_title: Aspose.ZIP for .NET API Referansı
description: SevenZipArchive inşaatçı. Yeni bir örneğini başlatır.SevenZipArchive girişleri için isteğe bağlı ayarlara sahip sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

Yeni bir örneğini başlatır.[`SevenZipArchive`](../) girişleri için isteğe bağlı ayarlara sahip sınıf.

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | Yeni eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) items. Belirtilmezse, şifrelemesiz LZMA sıkıştırması kullanılır. |

### Örnekler

Aşağıdaki örnek, tek bir dosyanın varsayılan ayarlarla nasıl sıkıştırılacağını gösterir: Şifrelemesiz LZMA sıkıştırma.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Ayrıca bakınız

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream) {#constructor_1}

Yeni bir örneğini başlatır.[`SevenZipArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public SevenZipArchive(Stream sourceStream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| sourceStream | Stream | Arşivin kaynağı. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | *sourceStream* aranmaz. |
| ArgumentNullException | *sourceStream* boş. |
| NotImplementedException | Arşiv birden fazla kodlayıcı içeriyor. Artık yalnızca LZMA sıkıştırması desteklenmektedir. |

### Notlar

Bu yapıcı herhangi bir girdiyi açmaz. Görmek[`ExtractToDirectory`](../extracttodirectory/) açma yöntemi.

### Örnekler

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Ayrıca bakınız

* class [SevenZipArchive](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## SevenZipArchive(string) {#constructor_2}

Yeni bir örneğini başlatır.[`SevenZipArchive`](../) class ve composes girişleri listesi arşivden çıkarılabilir.

```csharp
public SevenZipArchive(string path)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Arşiv dosyasının tam veya göreli yolu. |

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

Bu yapıcı herhangi bir girdiyi açmaz. Görmek[`ExtractToDirectory`](../extracttodirectory/) açma yöntemi.

### Örnekler

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Ayrıca bakınız

* class [SevenZipArchive](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchive/)
* toplantı [Aspose.Zip](../../../)


