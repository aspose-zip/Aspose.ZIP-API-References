---
title: "GetFormatInfo"
second_title: "Aspose.ZIP için .NET API Referansı"
description: 
type: docs
weight: 20
url: /tr/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

Biçim bilgilerini alır.

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String | Arşiv dosyasının dosya adı. |

### Dönüş Değeri

Arşiv formatı hakkında bilgi veya format algılanmadıysa null.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *fileName* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *fileName* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | Dosya *fileName*'e erişim reddedildi. |
| PathTooLongException | Belirtilen *fileName* sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden az olmalı ve dosya adları 260 karakterden az olmalıdır. |
| NotSupportedException | *fileName* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| IOException | Dosya açılırken bir G/Ç hatası oluştu. |

### Ayrıca Bakınız

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

Biçim bilgilerini alır.

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Arşiv dosyasının akışı. |

### Dönüş Değeri

Arşiv formatı hakkında bilgi veya format algılanmadıysa null.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *stream* null. |
| ArgumentException | *stream* arama yapılabilir değil. |

### Ayrıca Bakınız

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- DÜZENLEMEYİN: Aspose.Zip.dll için xmldocmd tarafından oluşturuldu -->
