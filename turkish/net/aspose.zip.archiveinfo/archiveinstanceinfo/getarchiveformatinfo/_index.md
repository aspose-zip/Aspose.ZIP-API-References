---
title: ArchiveInstanceInfo.GetArchiveFormatInfo
second_title: Aspose.ZIP for .NET API Referansı
description: ArchiveInstanceInfo yöntem. Arşiv biçimi bilgisini alır.
type: docs
weight: 50
url: /tr/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveformatinfo/
---
## GetArchiveFormatInfo(string) {#getarchiveformatinfo_1}

Arşiv biçimi bilgisini alır.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(string fileName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileName | String | Arşiv dosyasının dosya adı. |

### Geri dönüş değeri

Arşiv formatı hakkında bilgi veya format algılanmadıysa boş.

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

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* ad alanı [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* toplantı [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

Arşiv biçimi bilgisini alır.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Arşiv dosyasının akışı. |

### Geri dönüş değeri

Arşiv formatı hakkında bilgi veya format algılanmadıysa boş.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *stream* boş. |
| ArgumentException | *stream* aranmaz. |

### Ayrıca bakınız

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* ad alanı [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* toplantı [Aspose.Zip](../../../)


