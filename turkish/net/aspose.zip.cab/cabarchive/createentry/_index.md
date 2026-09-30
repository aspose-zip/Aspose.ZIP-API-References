---
title: "CabArchive.CreateEntry"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "CabArchive yöntemi. Arşiv içinde tek bir girdi oluşturur."
type: docs
weight: 40
url: /tr/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

Arşiv içinde tek bir girdi oluştur.

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Girişin adı. |
| yol | String | Yeni dosyanın tam nitelikli adı veya sıkıştırılacak göreli dosya adı. |
| newEntrySettings | CabEntrySettings | Eklenen [`CabEntry`](../../cabentry/) öğesi için kullanılan sıkıştırma ve şifreleme ayarları. |

### Dönüş Değeri

Cab giriş örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| InvalidOperationException | Arşiv çıkarma için hazırlanmıştır ve giriş eklenemez. |

## Açıklamalar

Giriş adı yalnızca *name* parametresi içinde ayarlanır. *path* parametresinde verilen dosya adı giriş adını etkilemez.

## Örnekler

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### Ayrıca Bakınız

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

Arşiv içinde tek bir girdi oluştur.

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Girişin adı. |
| kaynak | Akış | Giriş için giriş akışı. |
| newEntrySettings | CabEntrySettings | Eklenen [`CabEntry`](../../cabentry/) öğesi için kullanılan sıkıştırma ve şifreleme ayarları. |

### Dönüş Değeri

Cab giriş örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| InvalidOperationException | Arşiv çıkarma için hazırlanmıştır ve giriş eklenemez. |
| ArgumentNullException | *name* null. |

## Örnekler

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### Ayrıca Bakınız

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

Arşiv içinde tek bir girdi oluştur.

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Girişin adı. |
| fileInfo | FileInfo | Sıkıştırılacak dosyanın meta verileri. |
| newEntrySettings | CabEntrySettings | Eklenen [`CabEntry`](../../cabentry/) öğesi için kullanılan sıkıştırma ve şifreleme ayarları. |

### Dönüş Değeri

CAB giriş örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* yalnızca okunabilir veya bir dizindir. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| IOException | Dosya zaten açık. |
| FileNotFoundException | *fileInfo* bulunamayan bir dosyayı temsil eder. |
| SecurityException | Çağıran, *fileInfo*'a erişmek için gerekli izne sahip değil. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| InvalidOperationException | Arşiv çıkarma için hazırlanmıştır ve giriş eklenemez. |
| ArgumentNullException | *name* null. |

## Açıklamalar

Giriş adı yalnızca *name* parametresi içinde ayarlanır. *fileInfo* parametresinde verilen dosya adı giriş adını etkilemez.

## Örnekler

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### Ayrıca Bakınız

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

Arşiv içinde tek bir girdi oluştur.

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Girişin adı. |
| streamProvider | Func`1 | Giriş için giriş akışı sağlayan yöntem. |
| newEntrySettings | CabEntrySettings | Eklenen [`CabEntry`](../../cabentry/) öğesi için kullanılan sıkıştırma ve şifreleme ayarları. |

### Dönüş Değeri

CAB giriş örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Arşiv açma için oluşturulmuştur. - veya - Dosya sayısı sınıra ulaşmıştır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| ArgumentException | *name* null veya boş. |

## Örnekler

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### Ayrıca Bakınız

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


