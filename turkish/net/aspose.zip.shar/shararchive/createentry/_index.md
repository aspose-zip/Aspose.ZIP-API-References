---
title: SharArchive.CreateEntry
second_title: Aspose.ZIP for .NET API Referansı
description: SharArchive yöntem. Arşiv içinde tek giriş oluşturun.
type: docs
weight: 40
url: /tr/net/aspose.zip.shar/shararchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

Arşiv içinde tek giriş oluşturun.

```csharp
public SharEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| fileInfo | FileInfo | Sıkıştırılacak dosya veya klasörün meta verileri. |
| openImmediately | Boolean | Dosyayı hemen açarsanız doğrudur, aksi takdirde dosyayı arşive kaydederken açın. |

### Geri dönüş değeri

Paylaşım girişi örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *name* boş. |
| ArgumentException | *name* boş. |
| ArgumentNullException | *fileInfo* boş. |

### Notlar

Dosya ile hemen açılırsa*openImmediately*parametresi, arşiv atılana kadar bloke olur.

### Örnekler

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new SharArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.shar");
}
```

### Ayrıca bakınız

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* ad alanı [Aspose.Zip.Shar](../../shararchive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Arşiv içinde tek giriş oluşturun.

```csharp
public SharEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| sourcePath | String | Sıkıştırılacak dosyanın yolu. |
| openImmediately | Boolean | Dosyayı hemen açarsanız doğrudur, aksi takdirde dosyayı arşive kaydederken açın. |

### Geri dönüş değeri

Paylaşım girişi örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *sourcePath* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil. |
| ArgumentException | bu*sourcePath* boş, yalnızca beyaz boşluklar içeriyor veya geçersiz karakterler içeriyor. - veya - Dosya adı, bir parçası olarak*name*, 100 sembolü aşıyor. |
| UnauthorizedAccessException | dosyaya erişim*sourcePath* engellendi. |
| PathTooLongException | Belirtilen*sourcePath* , dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. - veya -*name* Shar için çok uzun. |
| NotSupportedException | dosya*sourcePath* dizenin ortasında iki nokta üst üste (:) içerir. |

### Notlar

Giriş adı yalnızca içinde ayarlanır*name* parametre. Verilen dosya adı*sourcePath* parametre giriş adını etkilemez.

Dosya ile hemen açılırsa*openImmediately*parametresi, arşiv atılana kadar bloke olur.

### Örnekler

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Ayrıca bakınız

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* ad alanı [Aspose.Zip.Shar](../../shararchive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Arşiv içinde tek giriş oluşturun.

```csharp
public SharEntry CreateEntry(string name, Stream source)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| source | Stream | Giriş için giriş akışı. |

### Geri dönüş değeri

Paylaşım girişi örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *name* boş. |
| ArgumentNullException | *source* boş. |
| ArgumentException | *name* boş. |

### Örnekler

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.shar");
}
```

### Ayrıca bakınız

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* ad alanı [Aspose.Zip.Shar](../../shararchive/)
* toplantı [Aspose.Zip](../../../)


