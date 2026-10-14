---
title: "AppleArchive.Save"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "AppleArchive yöntemi. Arşivi verilen akışa kaydeder."
type: docs
weight: 90
url: /tr/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

Arşivi sağlanan akışa kaydeder.

```csharp
public void Save(Stream output)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| çıktı | Akış | Hedef akış. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı. |
| ArgumentNullException | *output* `null`. |
| ArgumentException | *output* yazılabilir değil. |
| ArgumentOutOfRangeException | Yapılandırılmış LZ4 veya Zlib blok boyutu pozitif değil. |
| NotSupportedException | Sıkıştırma ayarları eksik veya desteklenmiyor, doğrudan birleştirme arama yapılabilir olmayan bir akış kullanıyor, ya da giriş/arşiv boyutu mevcut Apple Archive sınırlarını aşıyor. |

## Açıklamalar

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### Ayrıca Bakınız

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Arşivi sağlanan hedef dosyaya kaydeder.

```csharp
public void Save(string destinationFileName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationFileName | String | Oluşturulacak arşivin yolu. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı. |
| ArgumentException | *destinationFileName* geçersiz. |
| ArgumentNullException | *destinationFileName* `null`. |
| ArgumentOutOfRangeException | Yapılandırılmış LZ4 veya Zlib blok boyutu pozitif değil. |
| NotSupportedException | Sıkıştırma ayarları eksik veya desteklenmiyor, doğrudan birleştirme arama yapılabilir olmayan bir akış kullanıyor, ya da giriş/arşiv boyutu mevcut Apple Archive sınırlarını aşıyor. |

### Ayrıca Bakınız

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


