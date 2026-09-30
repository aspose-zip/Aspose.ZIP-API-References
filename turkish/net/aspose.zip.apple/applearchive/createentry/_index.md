---
title: "AppleArchive.CreateEntry"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "AppleArchive yöntemi. Arşiv içinde tek bir giriş oluşturur."
type: docs
weight: 60
url: /tr/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

Arşiv içinde tek bir giriş oluşturur.

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Girişin adı. |
| yol | String | Sıkıştırılacak dosyanın yolu. |
| openImmediately | Boolean | True, dosyayı hemen açmak için, aksi takdirde arşiv kaydedilirken dosyayı açar. |

### Dönüş Değeri

Apple Archive giriş örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı. |
| ArgumentException | *name* boş. |
| ArgumentNullException | *path* `null`. |

### Ayrıca Bakınız

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Arşiv içinde tek bir giriş oluşturur.

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Girişin adı. |
| kaynak | Akış | Giriş için giriş akışı. |

### Dönüş Değeri

Apple Archive giriş örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı. |
| ArgumentException | *name* boş. |
| ArgumentNullException | *source* `null` değerindedir. |

### Ayrıca Bakınız

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Arşiv içinde tek bir giriş oluşturur.

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Girişin adı. |
| fileInfo | FileInfo | Sıkıştırılacak dosyanın meta verileri. |
| openImmediately | Boolean | True, dosyayı hemen açmak için, aksi takdirde arşiv kaydedilirken dosyayı açar. |

### Dönüş Değeri

Apple Archive giriş örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı. |
| ArgumentException | *name* boş. |
| ArgumentNullException | *fileInfo* `null` değerindedir. |

### Ayrıca Bakınız

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


