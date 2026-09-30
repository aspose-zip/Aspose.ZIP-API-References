---
title: "Lz4Archive.Lz4Archive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Lz4Archive yapıcı. Çözümleme için hazırlanmış Lz4Archive sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

Çözümleme için hazırlanmış [`Lz4Archive`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | Akış | Arşivin kaynağı. |
| loadOptions | Lz4LoadOptions | Arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | *sourceStream*'den okunamıyor |
| ArgumentNullException | *sourceStream* null. |
| EndOfStreamException | *sourceStream* çok kısa. |
| InvalidDataException | *sourceStream*'in imzası yanlış. |
| ObjectDisposedException | Kaynak akış serbest bırakıldıysa fırlatılır. |
| IOException | Bir G/Ç hatası oluştu. |

## Açıklamalar

Bu yapıcı sıkıştırmayı açmaz. Açmak için [`Open`](../open/) yöntemine bakın.

## Örnekler

Bir akıştan arşivi açın ve bir `MemoryStream`'e çıkarın

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### Ayrıca Bakınız

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

[`Lz4Archive`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Arşiv dosyasının yolu. |
| loadOptions | Lz4LoadOptions | Arşivi yüklemek için seçenekler. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *path* null. |
| SecurityException | Çağıranın erişim için gerekli izni yok |
| ArgumentException | *path* boş, yalnızca boşluk karakterleri içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | *path* dosyasına erişim reddedildi. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| NotSupportedException | *path* konumundaki dosya, dizenin ortasında iki nokta üst üste (:) içeriyor. |
| EndOfStreamException | Dosya çok kısa. |
| InvalidDataException | Dosyadaki verinin imzası yanlış. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, örneğin eşlenmemiş bir sürücüde bulunması gibi. |
| FileNotFoundException | Dosya bulunamadı. |
| IOException | Dosya zaten açık. |

## Açıklamalar

Bu yapıcı sıkıştırmayı açmaz. Açmak için [`Open`](../open/) yöntemine bakın.

## Örnekler

Bir arşivi dosyadan yol ile aç ve onu bir `MemoryStream`'e çıkar

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### Ayrıca Bakınız

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

Sıkıştırma için hazırlanmış [`Lz4Archive`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ayarlar | Lz4ArchiveSetting | Bileşik arşivin ayarı. |

### Ayrıca Bakınız

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


