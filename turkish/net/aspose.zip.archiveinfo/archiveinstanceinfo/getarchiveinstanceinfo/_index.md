---
title: ArchiveInstanceInfo.GetArchiveInstanceInfo
second_title: Aspose.ZIP for .NET API Referansı
description: ArchiveInstanceInfo yöntem. Arşiv örneği bilgisini alır.
type: docs
weight: 10
url: /tr/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

Arşiv örneği bilgisini alır.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileName | String | Arşiv dosyasının dosya adı. |

### Geri dönüş değeri

Biçim algılanmadıysa arşiv örneği veya null hakkında bilgi.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *fileName* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil. |
| ArgumentException | bu*fileName* boş, yalnızca beyaz boşluklar içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | dosyaya erişim*fileName* engellendi. |
| PathTooLongException | Belirtilen*fileName* sistem tanımlı maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | dosya*fileName* dizenin ortasında iki nokta üst üste (:) içerir. |
| IOException | Dosya açılırken bir G/Ç hatası oluştu. |

### Ayrıca bakınız

* class [ArchiveInstanceInfo](../)
* ad alanı [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* toplantı [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

Arşiv örneği bilgisini alır.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Arşiv dosyasının akışı. |

### Geri dönüş değeri

Biçim algılanmadıysa arşiv örneği veya null hakkında bilgi.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *stream* boş. |
| ArgumentException | *stream* aranmaz. |

### Ayrıca bakınız

* class [ArchiveInstanceInfo](../)
* ad alanı [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* toplantı [Aspose.Zip](../../../)


