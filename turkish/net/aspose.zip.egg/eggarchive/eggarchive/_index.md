---
title: "EggArchive.EggArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "EggArchive yapıcı. Bir akıştan EggArchive sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

Bir akıştan [`EggArchive`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | EGG arşivi akışı. Akış okuma ve konumlandırma desteklemelidir. |
| loadOptions | EggArchiveLoadOptions | Arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *stream* null. |
| ArgumentException | *stream* okunabilir ve aranabilir değil. |

### Ayrıca Bakınız

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

Bir dosya yolundan [`EggArchive`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | EGG arşiv dosyasının yolu. |
| loadOptions | EggArchiveLoadOptions | Arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| FileNotFoundException | Dosya mevcut değil. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| IOException | Dosya zaten açık. |

### Ayrıca Bakınız

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


