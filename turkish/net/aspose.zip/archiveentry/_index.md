---
title: Class ArchiveEntry
second_title: Aspose.ZIP for .NET API Referansı
description: Aspose.Zip.ArchiveEntry sınıf. Arşivdeki tek dosyayı temsil eder.
type: docs
weight: 20
url: /tr/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

Arşivdeki tek dosyayı temsil eder.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Arşivdeki girişin yorumunu alır. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Sıkıştırılmış dosyanın boyutunu alır. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Sıkıştırma veya açma için ayarları alır. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Girdinin dizini temsil edip etmediğini gösteren bir değer alır. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Son değiştirilme tarihini ve saatini alır veya ayarlar. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Arşivdeki girişin adını alır. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Orijinal dosyanın boyutunu alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | Girdiyi sağlanan akışa çıkarır. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | Girdiyi sağlanan yolla dosya sistemine çıkarır. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Çıkarma için girişi açar ve sıkıştırılmış giriş içeriğiyle bir akış sağlar. |

## Olaylar

| İsim | Tanım |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Ham akışın bir kısmı sıkıştırıldığında yükselir. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Ham akışın bir kısmı çıkarıldığında yükselir. |

### Notlar

Yayınla`ArchiveEntry` örneğine[`ArchiveEntryEncrypted`](../archiveentryencrypted/) girişin şifrelenip şifrelenmediğini belirlemek için.

### Ayrıca bakınız

* interface [IArchiveFileEntry](../iarchivefileentry/)
* ad alanı [Aspose.Zip](../../aspose.zip/)
* toplantı [Aspose.Zip](../../)


