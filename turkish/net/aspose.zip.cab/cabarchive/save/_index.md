---
title: "CabArchive.Save"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "CabArchive yöntemi. Arşivi sağlanan akışa kaydeder"
type: docs
weight: 70
url: /tr/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

Arşivi sağlanan akışa kaydeder.

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| outputStream | Akış | Hedef akış. |
| saveOptions | CabSaveOptions | Arşiv kaydetme seçenekleri. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | *outputStream* yazılabilir ve aranabilir değil. |
| ObjectDisposedException | Arşiv serbest bırakıldı. |
| InvalidOperationException | Arşiv çıkarma için hazır ve kaydedilemez. |

## Açıklamalar

*outputStream* must be writable.

## Örnekler

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### Ayrıca Bakınız

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

Verilen hedef dosyaya arşivi kaydeder.

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationFileName | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacak. |
| saveOptions | CabSaveOptions | Arşiv kaydetme seçenekleri. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *destinationFileName* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *destinationFileName* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | Dosya *destinationFileName*'a erişim reddedildi. |
| PathTooLongException | Belirtilen *destinationFileName*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *destinationFileName* konumundaki dosya, dizenin ortasında bir iki nokta üst üste (:) içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| InvalidOperationException | Arşiv çıkarma için açıldı. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| IOException | Dosya zaten açık. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Açıklamalar

Bir arşivi yüklendiği aynı yola kaydetmek mümkündür. Ancak, bu yöntem geçici bir dosyaya kopyalama yaptığı için önerilmez.

## Örnekler

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Ayrıca Bakınız

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


