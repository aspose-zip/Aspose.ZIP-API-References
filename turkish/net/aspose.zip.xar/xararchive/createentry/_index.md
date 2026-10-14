---
title: "XarArchive.CreateEntry"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "XarArchive yöntemi. Arşiv içinde tek bir giriş oluşturur."
type: docs
weight: 40
url: /tr/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

Arşiv içinde tek bir girdi oluştur.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Girişin adı. |
| fileInfo | FileInfo | Sıkıştırılacak dosya veya klasörün meta verileri. |
| openImmediately | Boolean | True, dosyayı hemen açmak için, aksi takdirde arşiv kaydedilirken dosyayı açar. |
| compressionSettings | XarCompressionSettings | Eklenen [`XarEntry`](../../xarentry/) öğesi için kullanılan sıkıştırma ayarları. |

### Dönüş Değeri

Xar entry örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *name* null. |
| ArgumentException | *name* boş. |
| ArgumentNullException | *fileInfo* null. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Açıklamalar

*openImmediately* parametresiyle dosya hemen açılırsa, arşiv serbest bırakılana kadar engellenir.

## Örnekler

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### Ayrıca Bakınız

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

Arşiv içinde tek bir girdi oluştur.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Girişin adı. |
| sourcePath | String | Sıkıştırılacak dosyanın yolu. |
| openImmediately | Boolean | True, dosyayı hemen açmak için, aksi takdirde arşiv kaydedilirken dosyayı açar. |
| compressionSettings | XarCompressionSettings | Eklenen [`XarEntry`](../../xarentry/) öğesi için kullanılan sıkıştırma ayarları. |

### Dönüş Değeri

Xar entry örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *sourcePath* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *sourcePath* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. - veya - *name* parçası olan dosya adı 100 karakteri aşıyor. |
| UnauthorizedAccessException | Dosya *sourcePath* erişimi reddedildi. |
| PathTooLongException | Belirtilen *sourcePath*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden kısa olmalı ve dosya adları 260 karakterden kısa olmalıdır. - veya - *name* xar için çok uzun. |
| NotSupportedException | *sourcePath* konumundaki dosya, dizenin ortasında iki nokta (:) içeriyor. |
| InvalidOperationException | xar arşivi değiştirilemez. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Açıklamalar

Giriş adı yalnızca *name* parametresi içinde ayarlanır. *sourcePath* parametresinde verilen dosya adı giriş adını etkilemez.

*openImmediately* parametresiyle dosya hemen açılırsa, arşiv serbest bırakılana kadar engellenir.

## Örnekler

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### Ayrıca Bakınız

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

Arşiv içinde tek bir girdi oluştur.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Girişin adı. |
| kaynak | Akış | Giriş için giriş akışı. |
| compressionSettings | XarCompressionSettings | Eklenen [`XarEntry`](../../xarentry/) öğesi için kullanılan sıkıştırma ayarları. |

### Dönüş Değeri

Xar entry örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *name* null. |
| ArgumentNullException | *source* null. |
| ArgumentException | *name* boş. |
| InvalidOperationException | xar arşivi değiştirilemez. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Örnekler

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### Ayrıca Bakınız

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


