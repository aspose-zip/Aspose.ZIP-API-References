---
title: "AlzArchive.AlzArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "AlzArchive yapıcı. Bir akıştan AlzArchive sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.zip.alz/alzarchive/alzarchive/
---
## AlzArchive(Stream, AlzArchiveLoadOptions) {#constructor}

Bir akıştan yeni bir [`AlzArchive`](../) sınıfı örneği başlatır.

```csharp
public AlzArchive(Stream stream, AlzArchiveLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | ALZ arşiv akışı. Akış okuma ve arama (seeking) desteklemelidir. |
| loadOptions | AlzArchiveLoadOptions | Mevcut arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | akış null. |

### Ayrıca Bakınız

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)

---

## AlzArchive(string, AlzArchiveLoadOptions) {#constructor_1}

Bir dosya yolundan yeni bir [`AlzArchive`](../) sınıfı örneği başlatır.

```csharp
public AlzArchive(string filePath, AlzArchiveLoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | String | ALZ arşiv dosyasının yolu. |
| loadOptions | AlzArchiveLoadOptions | Mevcut arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | dosyaYolu null. |
| FileNotFoundException | Dosya mevcut değil. |

### Ayrıca Bakınız

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


