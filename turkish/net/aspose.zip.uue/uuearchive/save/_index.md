---
title: "UueArchive.Save"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "UueArchive yöntemi. Arşivi sağlanan akışa kaydeder"
type: docs
weight: 70
url: /tr/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

Arşivi sağlanan akışa kaydeder.

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| outputStream | Akış | Hedef akış. |
| saveOptions | UueSaveOptions | Arşivin kaydedilmesi için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| InvalidOperationException | Arşivlenecek veri kaynağı sağlanmadı. |
| ArgumentException | *outputStream* yazılabilir değil. |
| UnauthorizedAccessException | Dosya kaynağı yalnızca okunabilir veya bir dizindir. |
| DirectoryNotFoundException | Belirtilen dosya kaynağı yolu geçersiz, örneğin eşlenmemiş bir sürücüde olması gibi. |
| IOException | Dosya kaynağı zaten açık. |

## Açıklamalar

*outputStream* must be writable.

## Örnekler

Sıkıştırılmış veriyi http yanıt akışına yaz.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Ayrıca Bakınız

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

Arşivi sağlanan hedef dosyaya kaydeder.

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationFileName | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacak. |
| saveOptions | UueSaveOptions | Arşivin kaydedilmesi için seçenekler. |

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
| InvalidOperationException | Arşivlenecek veri kaynağı sağlanmadı. |

## Örnekler

Kodlanmış veriyi dosyaya yaz.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### Ayrıca Bakınız

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


