---
title: "XarArchive.Save"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "XarArchive yöntemi. Arşivi sağlanan hedef dosyaya kaydeder"
type: docs
weight: 80
url: /tr/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

Verilen hedef dosyaya arşivi kaydeder.

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationFileName | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacak. |
| saveOptions | XarSaveOptions | xar arşivini kaydetmek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *destinationFileName* null. |
| InvalidOperationException | xar arşivi değiştirilemez. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| IOException | Dosya açılırken bir G/Ç hatası oluştu. |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşar. |
| UnauthorizedAccessException | *destinationFileName* yalnızca okunabilir bir dosya olarak belirtildi. -veya- *destinationFileName* bir dizin olarak belirtildi. -veya- Çağıran gerekli izne sahip değil. |

### Ayrıca Bakınız

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

Arşivi sağlanan akışa kaydeder.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| çıktı | Akış | Hedef akış. |
| saveOptions | XarSaveOptions | xar arşivini kaydetmek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *output* null. |
| ArgumentException | *output*Yazılabilir/okunabilir değil veya arama yapılabilir değil. |
| InvalidOperationException | xar arşivi değiştirilemez. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

### Ayrıca Bakınız

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


