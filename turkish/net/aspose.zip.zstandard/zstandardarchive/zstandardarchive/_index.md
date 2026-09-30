---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "ZstandardArchive yapıcı. Sıkıştırma için hazırlanmış ZstandardArchive sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

Sıkıştırma için hazırlanmış [`ZstandardArchive`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ZstandardArchive()
```

## Örnekler

Aşağıdaki örnek bir dosyanın nasıl sıkıştırılacağını gösterir.

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### Ayrıca Bakınız

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

Açma için hazırlanmış [`ZstandardArchive`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | Akış | Arşivin kaynağı. |
| seçenekler | ZstandardLoadOptions | Arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Kaynak akış serbest bırakıldıysa fırlatılır. |
| EndOfStreamException | Akışın sonuna beklenmedik bir şekilde ulaşıldığında fırlatılır. |
| IOException | Bir G/Ç hatası oluştu. |
| InvalidDataException | Veri geçersiz veya bozuk olduğunda fırlatılır. |

## Açıklamalar

Bu yapıcı sıkıştırmayı açmaz. Açmak için [`Open`](../open/) yöntemine bakın.

## Örnekler

Bir akıştan arşivi açın ve bir `MemoryStream`'e çıkarın

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### Ayrıca Bakınız

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

[`ZstandardArchive`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Arşiv dosyasının yolu. |
| seçenekler | ZstandardLoadOptions | Arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıran, erişim için gerekli izne sahip değil. |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| EndOfStreamException | Akışın sonuna beklenmedik bir şekilde ulaşıldığında fırlatılır. |
| FileNotFoundException | Dosya bulunamadı. |
| IOException | Dosya zaten açık. |
| InvalidDataException | Veri geçersiz veya bozuk olduğunda fırlatılır. |

## Açıklamalar

Bu yapıcı sıkıştırmayı açmaz. Açmak için [`Open`](../open/) yöntemine bakın.

## Örnekler

Bir arşivi dosyadan yol ile aç ve onu bir `MemoryStream`'e çıkar

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### Ayrıca Bakınız

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


