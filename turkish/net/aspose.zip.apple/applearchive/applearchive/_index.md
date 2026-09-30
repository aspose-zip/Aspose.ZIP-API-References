---
title: "AppleArchive.AppleArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "AppleArchive yapıcı. Birleştirilmiş girişler için kullanılan ayarlarla AppleArchive sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

Yeni bir örnek başlatır [`AppleArchive`](../) sınıfının, birleştirilmiş girişler için kullanılan ayarlarla.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | Yeni bir Apple Archive oluştururken kullanılan ayarlar. |

### Ayrıca Bakınız

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

Yeni bir örnek başlatır [`AppleArchive`](../) sınıfının ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | Akış | Arşivin kaynağı. |
| loadOptions | AppleArchiveLoadOptions | Mevcut arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *sourceStream* null. |
| ArgumentException | *sourceStream* kaydırılamaz. |
| InvalidDataException | *sourceStream* geçerli bir Apple Archive değil. |
| EndOfStreamException | Akış, arşiv girişleri ayrıştırılırken beklenmedik şekilde sona eriyor. |

## Açıklamalar

Bu yapıcı herhangi bir girişi açmaz. Açmak için [`ExtractToDirectory`](../extracttodirectory/) ve [`Open`](../../applearchiveentry/open/) yöntemlerine bakın.

### Ayrıca Bakınız

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

Yeni bir örnek başlatır [`AppleArchive`](../) sınıfının ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Arşiv dosyasının tam nitelikli ya da göreceli yolu. |
| loadOptions | AppleArchiveLoadOptions | Mevcut arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| FileNotFoundException | Dosya bulunamadı. |
| InvalidDataException | *path* geçerli bir Apple Archive değil. |
| EndOfStreamException | Akış, arşiv girişleri ayrıştırılırken beklenmedik şekilde sona eriyor. |

## Açıklamalar

Bu yapıcı herhangi bir girişi açmaz. Açmak için [`ExtractToDirectory`](../extracttodirectory/) ve [`Open`](../../applearchiveentry/open/) yöntemlerine bakın.

### Ayrıca Bakınız

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


