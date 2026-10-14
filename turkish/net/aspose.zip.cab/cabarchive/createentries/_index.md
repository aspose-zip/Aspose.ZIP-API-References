---
title: "CabArchive.CreateEntries"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "CabArchive yöntemi. Belirtilen dizinden tüm dosyaları özyinelemeli olarak arşive ekler"
type: docs
weight: 30
url: /tr/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Belirtilen dizinden tüm dosyaları, özyinelemeli olarak, arşive ekler.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directory | DirectoryInfo | Sıkıştırılacak dizin. |
| includeRootDirectory | Boolean | Giriş yollarına kök dizin adının dahil edilip edilmeyeceğini gösterir. |

### Dönüş Değeri

Mevcut [`CabArchive`](../) örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *directory* null. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| DirectoryNotFoundException | *directory* bulunamıyor. |
| SecurityException | Çağıran, *directory*'e veya içeriğine erişmek için gerekli izne sahip değil. |
| UnauthorizedAccessException | *directory*'e veya dosyalarından birine erişim reddedildi. |
| IOException | Bir I/O hatası, *directory* erişilirken oluşur. |
| PathTooLongException | Oluşturulan giriş yolu, sistem tarafından tanımlanan maksimum uzunluğu aşıyor. |
| InvalidOperationException | Arşiv çıkarma için hazırlanmıştır ve giriş eklenemez. |

## Örnekler

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### Ayrıca Bakınız

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Belirtilen dizin yolundan tüm dosyaları özyinelemeli olarak arşive ekler.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceDirectory | String | Sıkıştırılacak dizin yolu. |
| includeRootDirectory | Boolean | Giriş yollarına kök dizin adının dahil edilip edilmeyeceğini gösterir. |

### Dönüş Değeri

Mevcut [`CabArchive`](../) örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| ArgumentNullException | *sourceDirectory* null. |
| DirectoryNotFoundException | *sourceDirectory* bulunamıyor. |
| SecurityException | Çağıran, *sourceDirectory*'e erişmek için gerekli izne sahip değil. |
| UnauthorizedAccessException | *sourceDirectory*'e erişim reddedildi. |
| PathTooLongException | Belirtilen *sourceDirectory* sistem tarafından tanımlanan maksimum uzunluğu aşıyor. |
| ArgumentException | *sourceDirectory* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| IOException | Bir I/O hatası, *sourceDirectory* erişilirken oluşur. |
| InvalidOperationException | Arşiv çıkarma için hazırlanmıştır ve giriş eklenemez. |

## Örnekler

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### Ayrıca Bakınız

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


