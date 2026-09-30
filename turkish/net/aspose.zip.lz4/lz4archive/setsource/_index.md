---
title: "Lz4Archive.SetSource"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Lz4Archive yöntemi. Arşiv içinde sıkıştırılacak içeriği ayarlar"
type: docs
weight: 70
url: /tr/net/aspose.zip.lz4/lz4archive/setsource/
---
## SetSource(Stream) {#setsource_2}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(Stream source)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Akış | Arşiv için giriş akışı. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Arşiv çıkarma için hazırlanmıştır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Örnekler

```csharp
using (var archive = new Lz4Archive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz4");
}
```

### Ayrıca Bakınız

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

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
| InvalidOperationException | Arşiv çıkarma için hazırlanmıştır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Örnekler

Bir akıştan arşivi açın ve bir `MemoryStream`'e çıkarın

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz4");
}
```

### Ayrıca Bakınız

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tarArchive | TarArchive | Sıkıştırılacak tar arşivi. |
| biçim | TarFormat | Tar başlık biçimini tanımlar. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| InvalidOperationException | Bu arşiv çıkarma için hazırlanmıştır. |

## Açıklamalar

Ortak tar.lz4 arşivi oluşturmak için bu yöntemi kullanın.

## Örnekler

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var lz4Archive = new Lz4Archive())
    {
        lz4Archive.SetSource(tarArchive);
        lz4Archive.Save("archive.tar.lz4");
    }
}
```

### Ayrıca Bakınız

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Arşiv içinde sıkıştırılacak içeriği ayarlar.

```csharp
public void SetSource(string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Sıkıştırılacak dosyanın yolu. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıranın erişim için gerekli izni yok |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| InvalidOperationException | Bu arşiv çıkarma için hazırlanmıştır. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Örnekler

Bir arşivi dosyadan yol ile aç ve onu bir `MemoryStream`'e çıkar

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Ayrıca Bakınız

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


