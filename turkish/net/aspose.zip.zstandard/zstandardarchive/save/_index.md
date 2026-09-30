---
title: "ZstandardArchive.Save"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "ZstandardArchive yöntemi. Arşivi sağlanan akışa kaydeder"
type: docs
weight: 60
url: /tr/net/aspose.zip.zstandard/zstandardarchive/save/
---
## Save(Stream, ZstandardSaveOptions) {#save_1}

Arşivi sağlanan akışa kaydeder.

```csharp
public void Save(Stream outputStream, ZstandardSaveOptions settings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| outputStream | Akış | Hedef akış. |
| ayarlar | ZstandardSaveOptions | Arşiv oluşturulması için isteğe bağlı ayarlar. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| ArgumentException | *outputStream* yazılabilir değil. |
| InvalidOperationException | Kaynak sağlanmadı. |

## Açıklamalar

*outputStream* must be writable.

## Örnekler

Sıkıştırılmış veriyi http yanıt akışına yaz.

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Ayrıca Bakınız

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZstandardSaveOptions) {#save_2}

Verilen hedef dosyaya arşivi kaydeder.

```csharp
public void Save(string destinationFileName, ZstandardSaveOptions settings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationFileName | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacak. |
| ayarlar | ZstandardSaveOptions | Arşiv oluşturulması için isteğe bağlı ayarlar. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| ArgumentNullException | *destinationFileName* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *destinationFileName* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | Dosya *destinationFileName*'a erişim reddedildi. |
| PathTooLongException | Belirtilen *destinationFileName*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *destinationFileName* konumundaki dosya, dizenin ortasında bir iki nokta üst üste (:) içeriyor. |
| İstisna | Çalışma zamanı hatası oluştuğunda atılır. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, (örneğin, eşlenmemiş bir sürücüde bulunması). |
| IOException | Dosya açılırken bir G/Ç hatası oluştu. |
| InvalidOperationException | Kaynak sağlanmadı. |

## Örnekler

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.zst");
}
```

### Ayrıca Bakınız

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo, ZstandardSaveOptions) {#save}

Verilen hedef dosyaya arşivi kaydeder.

```csharp
public void Save(FileInfo destination, ZstandardSaveOptions settings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | FileInfo | FileInfo, hedef akış olarak açılacak. |
| ayarlar | ZstandardSaveOptions | Arşiv oluşturulması için isteğe bağlı ayarlar. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| SecurityException | Çağıranın *destination* açmak için gerekli izni yok. |
| ArgumentException | Dosya yolu boş veya yalnızca boşluk içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| UnauthorizedAccessException | Dosya yolu yalnızca okunabilir veya bir dizin. |
| ArgumentNullException | *destination* null. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| IOException | Dosya zaten açık. |
| InvalidOperationException | Kaynak sağlanmadı. |

## Örnekler

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.zst"));
}
```

### Ayrıca Bakınız

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


