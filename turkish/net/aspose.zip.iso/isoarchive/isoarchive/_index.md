---
title: "IsoArchive.IsoArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "IsoArchive yapıcı. IsoArchive sınıfının yeni bir örneğini başlatır ve yeni dosya ve dizinler eklemek için boş bir ISO arşivi oluşturur."
type: docs
weight: 10
url: /tr/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

[`IsoArchive`](../) sınıfının yeni bir örneğini başlatır ve yeni dosya ve dizinler eklemek için boş bir ISO arşivi oluşturur.

```csharp
public IsoArchive()
```

## Örnekler

Aşağıdaki örnek, yeni bir boş ISO arşivi oluşturmayı ve dosyaları eklemeyi gösterir:

```csharp
// Yeni bir boş ISO arşivi oluştur
using(IsoArchive isoArchive = new IsoArchive())
{
    // Dosyaları ISO arşivine ekle
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // ISO arşivini bir dosyaya kaydet
    isoArchive.Save("new_archive.iso");
}
```

### Ayrıca Bakınız

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

[`IsoArchive`](../) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | Akış | Arşivin kaynağı. Kaydırılabilir olmalıdır. |
| loadOptions | IsoLoadOptions | Arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *sourceStream* null. |
| ArgumentException | *sourceStream* kaydırılamaz. |
| InvalidDataException | *sourceStream* geçerli bir ISO arşivi değil. |
| ObjectDisposedException | Kaynak akış serbest bırakıldıysa fırlatılır. |
| EndOfStreamException | Akışın sonuna beklenmedik bir şekilde ulaşıldığında fırlatılır. |
| IOException | Bir G/Ç hatası oluştu. |
| NotSupportedException | Akış okuma desteklemiyor. |

## Açıklamalar

Bu yapıcı hiçbir girişi açmaz.

## Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Ayrıca Bakınız

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

[`IsoArchive`](../) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Arşiv dosyasının yolu. |
| loadOptions | IsoLoadOptions | Arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| IOException | Dosya zaten açık. |
| EndOfStreamException | Dosya çok kısa. |
| InvalidDataException | Veri geçersiz veya bozuk olduğunda fırlatılır. |

## Açıklamalar

Bu yapıcı hiçbir girişi açmaz.

## Örnekler

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Ayrıca Bakınız

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


