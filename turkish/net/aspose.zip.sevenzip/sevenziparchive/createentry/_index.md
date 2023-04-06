---
title: SevenZipArchive.CreateEntry
second_title: Aspose.ZIP for .NET API Referansı
description: SevenZipArchive yöntem. Arşiv içinde tek giriş oluşturun.
type: docs
weight: 50
url: /tr/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

Arşiv içinde tek giriş oluşturun.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| fileInfo | FileInfo | Sıkıştırılacak dosyanın meta verileri. |
| openImmediately | Boolean | Dosyayı hemen açarsanız doğrudur, aksi takdirde dosyayı arşive kaydederken açın. |
| newEntrySettings | SevenZipEntrySettings | Eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) öğe. |

### Geri dönüş değeri

Yedi Zip girişi örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* salt okunurdur veya bir dizindir. |
| DirectoryNotFoundException | Eşlenmemiş bir sürücüde olmak gibi, belirtilen yol geçersiz. |
| IOException | Dosya zaten açık. |

### Notlar

Giriş adı yalnızca içinde ayarlanır*name* parametre. Verilen dosya adı*fileInfo* parametre giriş adını etkilemez.

Dosya ile hemen açılırsa*openImmediately* parametresi, arşiv kaydedilene kadar bloke olur.

### Örnekler

Her biri farklı parolalarla şifrelenmiş girişlerle arşiv oluşturun.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### Ayrıca bakınız

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

Arşiv içinde tek giriş oluşturun.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| source | Stream | Giriş için giriş akışı. |
| newEntrySettings | SevenZipEntrySettings | Eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) öğe. |
| fileInfo | FileSystemInfo | Sıkıştırılacak dosya veya klasörün meta verileri. |

### Geri dönüş değeri

SevenZip giriş örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| InvalidOperationException | İkisi birden*source* Ve*fileInfo* boş veya*source*boş ve*fileInfo* dizin anlamına gelir. |

### Notlar

Giriş adı yalnızca içinde ayarlanır*name* parametre. Verilen dosya adı*fileInfo* parametre giriş adını etkilemez.

*fileInfo* başvurabilirDirectoryInfo giriş dizin ise.

### Örnekler

LZMA2 sıkıştırılmış şifreli giriş ile arşiv oluşturun.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### Ayrıca bakınız

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

Arşiv içinde tek giriş oluşturun.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| source | Stream | Giriş için giriş akışı. |
| newEntrySettings | SevenZipEntrySettings | Eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) öğe. |

### Geri dönüş değeri

Zip girişi örneği.

### Örnekler

LZMA2 sıkıştırma ve tüm girişlerin şifrelenmesi ile 7z arşivi oluşturun.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### Ayrıca bakınız

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

Arşiv içinde tek giriş oluşturun.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| path | String | Yeni dosyanın tam adı veya sıkıştırılacak ilgili dosya adı. |
| openImmediately | Boolean | Dosyayı hemen açarsanız doğrudur, aksi takdirde dosyayı arşive kaydederken açın. |
| newEntrySettings | SevenZipEntrySettings | Eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) öğe. |

### Geri dönüş değeri

Zip girişi örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *path* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil. |
| ArgumentException | bu*path* boş, yalnızca beyaz boşluklar içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | dosyaya erişim*path* engellendi. |
| PathTooLongException | Belirtilen*path*, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | dosya*path* dizenin ortasında iki nokta üst üste (:) içerir. |

### Notlar

Giriş adı yalnızca içinde ayarlanır*name* parametre. Verilen dosya adı*path* parametre giriş adını etkilemez.

Dosya ile hemen açılırsa*openImmediately* parametresi, arşiv kaydedilene kadar bloke olur.

### Örnekler

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Ayrıca bakınız

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* ad alanı [Aspose.Zip.SevenZip](../../sevenziparchive/)
* toplantı [Aspose.Zip](../../../)


