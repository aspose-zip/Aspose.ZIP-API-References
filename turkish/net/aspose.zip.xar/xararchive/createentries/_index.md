---
title: "XarArchive.CreateEntries"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "XarArchive yöntemi. Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler"
type: docs
weight: 30
url: /tr/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceDirectory | String | Sıkıştırılacak dizin. |
| compressionSettings | Boolean | Eklenen [`XarEntry`](../../xarentry/) öğeleri için kullanılan sıkıştırma ayarları. |
| includeRootDirectory | XarCompressionSettings | Kök dizini kendisi dahil edilip edilmeyeceğini gösterir. |

### Dönüş Değeri

Xar entry örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *sourceDirectory* null. |
| SecurityException | Çağıran, *sourceDirectory*'e erişmek için gerekli izne sahip değil. |
| ArgumentException | *sourceDirectory* \" , &lt;, &gt;, veya &#x7C; gibi geçersiz karakterler içeriyor. |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden kısa olmalı ve dosya adları 260 karakterden kısa olmalıdır. Belirtilen yol, dosya adı veya her ikisi çok uzun. |
| IOException | *sourceDirectory* bir dosyayı temsil eder, bir dizini değil. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Örnekler

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### Ayrıca Bakınız

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directory | DirectoryInfo | Sıkıştırılacak dizin. |
| compressionSettings | Boolean | Eklenen [`XarEntry`](../../xarentry/) öğeleri için kullanılan sıkıştırma ayarları. |
| includeRootDirectory | XarCompressionSettings | Kök dizini kendisi dahil edilip edilmeyeceğini gösterir. |

### Dönüş Değeri

Xar entry örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *directory* null. |
| SecurityException | Çağıran, *directory* erişimi için gerekli izne sahip değil. |
| IOException | *directory* bir dosyayı temsil eder, bir dizini değil. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Örnekler

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### Ayrıca Bakınız

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


