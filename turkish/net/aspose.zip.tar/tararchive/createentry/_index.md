---
title: TarArchive.CreateEntry
second_title: Aspose.ZIP for .NET API Referansı
description: TarArchive yöntem. Arşiv içinde tek giriş oluşturun.
type: docs
weight: 80
url: /tr/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Arşiv içinde tek giriş oluşturun.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| source | Stream | Giriş için giriş akışı. |
| fileInfo | FileSystemInfo | Sıkıştırılacak dosya veya klasörün meta verileri. |

### Geri dönüş değeri

Tar girişi örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| PathTooLongException | *name* IEEE 1003.1-1998 standardına göre katran için çok uzun. |
| ArgumentException | dosya adı, bir parçası olarak*name*, 100 sembolü aşıyor. |

### Notlar

Giriş adı yalnızca içinde ayarlanır*name* parametre. Verilen dosya adı*fileInfo* parametre giriş adını etkilemez.

*fileInfo* başvurabilirDirectoryInfo giriş dizin ise.

### Örnekler

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### Ayrıca bakınız

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Arşiv içinde tek giriş oluşturun.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| fileInfo | FileInfo | Sıkıştırılacak dosya veya klasörün meta verileri. |
| openImmediately | Boolean | Dosyayı hemen açarsanız doğrudur, aksi takdirde dosyayı arşive kaydederken açın. |

### Geri dönüş değeri

Tar girişi örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| PathTooLongException | *name* IEEE 1003.1-1998 standardına göre katran için çok uzun. |
| ArgumentException | dosya adı, bir parçası olarak*name*, 100 sembolü aşıyor. |

### Notlar

Giriş adı yalnızca içinde ayarlanır*name* parametre. Verilen dosya adı*fileInfo* parametre giriş adını etkilemez.

*fileInfo* başvurabilirDirectoryInfo giriş dizin ise.

Dosya ile hemen açılırsa*openImmediately*parametresi, arşiv atılana kadar bloke olur.

### Örnekler

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### Ayrıca bakınız

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Arşiv içinde tek giriş oluşturun.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| path | String | Sıkıştırılacak dosyanın yolu. |
| openImmediately | Boolean | Dosyayı hemen açarsanız doğrudur, aksi takdirde dosyayı arşive kaydederken açın. |

### Geri dönüş değeri

Tar girişi örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *path* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil. |
| ArgumentException | bu*path* boş, yalnızca beyaz boşluklar içeriyor veya geçersiz karakterler içeriyor. - veya - Dosya adı, bir parçası olarak*name*, 100 sembolü aşıyor. |
| UnauthorizedAccessException | dosyaya erişim*path* engellendi. |
| PathTooLongException | Belirtilen*path* , dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. - veya -*name* IEEE 1003.1-1998 standardına göre katran için çok uzun. |
| NotSupportedException | dosya*path* dizenin ortasında iki nokta üst üste (:) içerir. |

### Notlar

Giriş adı yalnızca içinde ayarlanır*name* parametre. Verilen dosya adı*path* parametre giriş adını etkilemez.

Dosya ile hemen açılırsa*openImmediately*parametresi, arşiv atılana kadar bloke olur.

### Örnekler

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### Ayrıca bakınız

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)


