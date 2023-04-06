---
title: Archive.CreateEntry
second_title: Aspose.ZIP for .NET API Referansı
description: Archive yöntem. Arşiv içinde tek giriş oluşturun.
type: docs
weight: 50
url: /tr/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

Arşiv içinde tek giriş oluşturun.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| path | String | Yeni dosyanın tam adı veya sıkıştırılacak ilgili dosya adı. |
| openImmediately | Boolean | Dosyayı hemen açarsanız doğrudur, aksi takdirde dosyayı arşive kaydederken açın. |
| newEntrySettings | ArchiveEntrySettings | Eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`ArchiveEntry`](../../archiveentry/) öğe. |

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
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Ayrıca bakınız

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ad alanı [Aspose.Zip](../../archive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

Arşiv içinde tek giriş oluşturun.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| source | Stream | Giriş için giriş akışı. |
| newEntrySettings | ArchiveEntrySettings | Eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`ArchiveEntry`](../../archiveentry/) öğe. |

### Geri dönüş değeri

Zip girişi örneği.

### Örnekler

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### Ayrıca bakınız

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ad alanı [Aspose.Zip](../../archive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

Arşiv içinde tek giriş oluşturun.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| fileInfo | FileInfo | Sıkıştırılacak dosyanın meta verileri. |
| openImmediately | Boolean | Dosyayı hemen açarsanız doğrudur, aksi takdirde dosyayı arşive kaydederken açın. |
| newEntrySettings | ArchiveEntrySettings | Eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`ArchiveEntry`](../../archiveentry/) öğe. |

### Geri dönüş değeri

Zip girişi örneği.

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

Her biri farklı şifreleme yöntemleri ve parolalarla şifrelenmiş girişlerle arşiv oluşturun.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### Ayrıca bakınız

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ad alanı [Aspose.Zip](../../archive/)
* toplantı [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

Arşiv içinde tek giriş oluşturun.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Girişin adı. |
| source | Stream | Giriş için giriş akışı. |
| newEntrySettings | ArchiveEntrySettings | Eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`ArchiveEntry`](../../archiveentry/) öğe. |
| fileInfo | FileSystemInfo | Sıkıştırılacak dosya veya klasörün meta verileri. |

### Geri dönüş değeri

Zip girişi örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| InvalidOperationException | İkisi birden*source* Ve*fileInfo* boş veya*source*boş ve*fileInfo* dizin anlamına gelir. |

### Notlar

Giriş adı yalnızca içinde ayarlanır*name* parametre. Verilen dosya adı*fileInfo* parametre giriş adını etkilemez.

*fileInfo* başvurabilirDirectoryInfo giriş dizin ise.

### Örnekler

Şifreli giriş ile arşiv oluşturun.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### Ayrıca bakınız

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ad alanı [Aspose.Zip](../../archive/)
* toplantı [Aspose.Zip](../../../)


