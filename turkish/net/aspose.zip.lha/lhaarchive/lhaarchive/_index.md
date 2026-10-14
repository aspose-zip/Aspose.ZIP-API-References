---
title: "LhaArchive.LhaArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "LhaArchive yapıcı. LhaArchive sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur"
type: docs
weight: 10
url: /tr/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

Yeni bir [`LhaArchive`](../) sınıf örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | Akış | Arşivin kaynağı. |
| loadOptions | LhaLoadOptions | Mevcut arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *sourceStream* null. |
| ArgumentException | *sourceStream* arama yapılamaz. |
| InvalidDataException | Uygun olmayan veri bulundu. |
| EndOfStreamException | Akışın sonuna, beklenen bayt sayısı okunmadan önce ulaşıldığında atılır. |
| ObjectDisposedException | Nesne atıldıktan sonra (dispose edildiğinde) fırlatılır. |

## Açıklamalar

Bu yapıcı hiçbir girdiyi açmaz. Açmak için [`Extract`](../../lhaarchiveentry/extract/) yöntemine bakın.

### Ayrıca Bakınız

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

Yeni bir [`LhaArchive`](../) sınıf örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Arşiv dosyasının tam nitelikli ya da göreceli yolu. |
| loadOptions | LhaLoadOptions | Mevcut arşivi yüklemek için seçenekler. |

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
| EndOfStreamException | Akışın sonuna, beklenen bayt sayısı okunmadan önce ulaşıldığında atılır. |
| ObjectDisposedException | Nesne atıldıktan sonra (dispose edildiğinde) fırlatılır. |

## Açıklamalar

Bu yapıcı hiçbir girdiyi açmaz. Açmak için [`Extract`](../../lhaarchiveentry/extract/) yöntemine bakın.

## Örnekler

Aşağıdaki örnek bir arşivi çıkarır, ardından ilk girdiyi bir `MemoryStream`'e açar.

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Ayrıca Bakınız

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


