---
title: "UueArchive.SetSource"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "UueArchive yöntemi. Arşiv içinde kodlanacak içeriği ayarlar"
type: docs
weight: 80
url: /tr/net/aspose.zip.uue/uuearchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Arşiv içinde kodlanacak içeriği ayarlar.

```csharp
public void SetSource(Stream source)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Akış | Arşiv için giriş akışı. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Örnekler

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.uue");
}
```

### Ayrıca Bakınız

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileInfo | FileInfo | Sıkıştırılacak dosyaya referans. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Örnekler

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.uue");
}
```

### Ayrıca Bakınız

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Arşiv içinde kodlanacak içeriği ayarlar.

```csharp
public void SetSource(string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Kodlanacak dosyanın yolu. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |

## Örnekler

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### Ayrıca Bakınız

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


