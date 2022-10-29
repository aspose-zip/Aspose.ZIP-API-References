---
title: Extract
second_title: Aspose.ZIP for .NET API Referansı
description: Z arşivini bir akışa çıkarır.
type: docs
weight: 30
url: /tr/net/aspose.zip.z/zarchive/extract/
---
## Extract(Stream) {#extract_1}

Z arşivini bir akışa çıkarır.

```csharp
public void Extract(Stream destination)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| destination | Stream | Sıkıştırılmış verileri depolamak için akış. |

### istisnalar

| istisna | şart |
| --- | --- |
| InvalidDataException | Veriler sıkıştırılamaz. |

### Örnekler

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new ZArchive(zFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### Ayrıca bakınız

* class [ZArchive](../../zarchive)
* ad alanı [Aspose.Zip.Z](../../zarchive)
* toplantı [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract}

Z arşivini bir dosyaya çıkarır.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileInfo | FileInfo | Sıkıştırılmış verileri depolamak için FileInfo. |

### istisnalar

| istisna | şart |
| --- | --- |
| SecurityException | Arayan, cihazı açmak için gerekli izne sahip değil.*fileInfo*. |
| ArgumentException | Dosya yolu boş veya yalnızca beyaz boşluklar içeriyor. |
| FileNotFoundException | Dosya bulunamadı. |
| UnauthorizedAccessException | Dosya yolu salt okunurdur veya bir dizindir. |
| ArgumentNullException | *fileInfo* boş. |
| DirectoryNotFoundException | Belirtilen yol, eşlenmemiş bir sürücüde olmak gibi geçersiz. |
| IOException | Dosya zaten açık. |
| InvalidDataException | Veriler sıkıştırılamaz. |

### Örnekler

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Ayrıca bakınız

* class [ZArchive](../../zarchive)
* ad alanı [Aspose.Zip.Z](../../zarchive)
* toplantı [Aspose.Zip](../../../)

---

## Extract(string) {#extract_2}

Z arşivini yola göre bir dosyaya çıkarır.

```csharp
public void Extract(string path)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Sıkıştırılmış verileri depolayacak dosyanın yolu. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *path* boş. |
| SecurityException | Arayan, erişim için gerekli izne sahip değil |
| ArgumentException | bu*path* boş, yalnızca boşluk içeriyor veya geçersiz karakterler içeriyor. |
| UnauthorizedAccessException | Dosyaya erişim*path* engellendi. |
| PathTooLongException | Belirtilmiş*path*, dosya adı veya her ikisi de sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden ve dosya adları 260 karakterden az olmalıdır. |
| NotSupportedException | Dosya*path* dizenin ortasında iki nokta üst üste (:) içerir. |
| InvalidDataException | Veriler sıkıştırılamaz. |

### Örnekler

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Ayrıca bakınız

* class [ZArchive](../../zarchive)
* ad alanı [Aspose.Zip.Z](../../zarchive)
* toplantı [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->