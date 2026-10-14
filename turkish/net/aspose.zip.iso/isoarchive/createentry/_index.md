---
title: "IsoArchive.CreateEntry"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "IsoArchive yöntemi. Bir dosyayı ISO görüntüsüne ekler"
type: docs
weight: 40
url: /tr/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

ISO görüntüsüne bir dosya ekler.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | ISO içindeki dosyanın yolu. |
| filePath | String | Dosyanın yolu. |

### Dönüş Değeri

ISO girişi oluşturuldu.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *filePath* null. |
| ArgumentException | *filePath* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *filePath* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *filePath* sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *filePath* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| IOException | Dosya açılırken bir G/Ç hatası oluştu. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, (örneğin, eşlenmemiş bir sürücüde bulunması). |
| FileNotFoundException | Belirtilen *filePath* dosyası bulunamadı. |
| InvalidOperationException | Arşiv düzenleme modunda değil. |

### Ayrıca Bakınız

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

ISO görüntüsüne bir dosya ekler.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | ISO içindeki dosyanın yolu. |
| kaynak | Akış | Dosya verilerini içeren akış. |

### Dönüş Değeri

ISO girişi oluşturuldu.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| ArgumentNullException | *name* veya *source* null olduğunda atılır. |
| InvalidOperationException | Arşiv düzenleme modunda değil. |

### Ayrıca Bakınız

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

ISO görüntüsüne bir dosya ekler.

```csharp
public IsoEntry CreateEntry(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | ISO içindeki dizinin yolu. |

### Dönüş Değeri

ISO girişi oluşturuldu.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | `name` null veya boş. |
| InvalidOperationException | Arşiv çıkarma için açıldı. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

### Ayrıca Bakınız

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


