---
title: Class SevenZipArchiveEntry
second_title: Aspose.ZIP for .NET API Referansı
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry sınıf. 7z arşivindeki tek dosyayı temsil eder.
type: docs
weight: 670
url: /tr/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

7z arşivindeki tek dosyayı temsil eder.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Sıkıştırılmış dosyanın boyutunu alır. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Sıkıştırma veya açma için ayarları alır. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Girdinin dizini temsil edip etmediğini gösteren bir değer alır. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Son değiştirilme tarihini ve saatini alır. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Arşivdeki girişin adını alır. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Orijinal dosyanın boyutunu alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | Girdiyi sağlanan akışa çıkarır. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | Girdiyi sağlanan yolla dosya sistemine çıkarır. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Çıkarma için girişi açar ve giriş içeriğine sahip bir akış sağlar. |

## Olaylar

| İsim | Tanım |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Ham akışın bir kısmı sıkıştırıldığında yükselir. |

### Notlar

Yayınla`SevenZipArchiveEntry` örneğine[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) girişin şifrelenip şifrelenmediğini belirlemek için.

### Ayrıca bakınız

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* ad alanı [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* toplantı [Aspose.Zip](../../)


