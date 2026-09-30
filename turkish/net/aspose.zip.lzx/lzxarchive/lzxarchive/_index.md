---
title: "LzxArchive.LzxArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "LzxArchive yapıcı. LzxArchive sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur"
type: docs
weight: 10
url: /tr/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

[`LzxArchive`](../) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| extractionSource | Akış | Arşivin kaynağı. |
| loadOptions | LzxLoadOptions | Mevcut arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *extractionSource* null. |
| ArgumentException | *extractionSource* arama desteklemiyor. |
| InvalidDataException | Arşiv için yanlış imza. - veya - Dosya bir LZX arşivi değil. |
| NotImplementedException | Lzx arşivi birleştirilmiş girişler içeriyor. |
| EndOfStreamException | *extractionSource* akışı çok kısa. |
| ObjectDisposedException | Akış kapatıldıysa fırlatılır. |
| IOException | Bir G/Ç hatası oluştu. |

## Açıklamalar

Bu yapıcı herhangi bir girişi açmaz. Açmak için [`Extract`](../../lzxarchiveentry/extract/) metoduna bakın.

### Ayrıca Bakınız

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

[`LzxArchive`](../) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Arşiv dosyasının tam nitelikli ya da göreceli yolu. |
| loadOptions | LzxLoadOptions | Mevcut arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| IOException | Dosya zaten açık. |
| InvalidDataException | Dosya bozulmuş. |
| NotImplementedException | Lzx arşivi birleştirilmiş girişler içeriyor. |
| EndOfStreamException | Dosya çok kısa. |
| ObjectDisposedException | Akış kapatıldıysa fırlatılır. |

## Açıklamalar

Bu yapıcı herhangi bir girişi açmaz. Açmak için [`Extract`](../../lzxarchiveentry/extract/) metoduna bakın.

## Örnekler

Aşağıdaki örnek bir arşivi çıkarır, ardından ilk girdiyi bir `MemoryStream`'e açar.

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Ayrıca Bakınız

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


