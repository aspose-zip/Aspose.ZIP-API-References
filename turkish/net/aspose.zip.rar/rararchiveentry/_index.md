---
title: Class RarArchiveEntry
second_title: Aspose.ZIP for .NET API Referansı
description: Aspose.Zip.Rar.RarArchiveEntry sınıf. Arşivdeki tek dosyayı temsil eder.
type: docs
weight: 320
url: /tr/net/aspose.zip.rar/rararchiveentry/
---
## RarArchiveEntry class

Arşivdeki tek dosyayı temsil eder.

```csharp
public abstract class RarArchiveEntry : IArchiveFileEntry
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | Sıkıştırılmış dosyanın boyutunu alır. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | Oluşturma tarihini ve saatini alır. |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | Girdinin dizini temsil edip etmediğini gösteren bir değer alır. |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | Son erişim tarihini ve saatini alır. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | Son değiştirilme tarihini ve saatini alır. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | Arşivdeki girişin adını alır. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | Orijinal dosyanın boyutunu alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract_1)(Stream, string) | Girdiyi sağlanan akışa çıkarır. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract)(string, string) | Girdiyi sağlanan yolla dosya sistemine çıkarır. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | Çıkarma için girişi açar ve sıkıştırılmış giriş içeriğiyle bir akış sağlar. |

## Olaylar

| İsim | Tanım |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | Ham akışın bir kısmı çıkarıldığında yükselir. |

### Notlar

Bir yayınla`RarArchiveEntry` örneğine[`RarArchiveEntryEncrypted`](../rararchiveentryencrypted/) girişin şifrelenip şifrelenmediğini belirlemek için.

### Ayrıca bakınız

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* ad alanı [Aspose.Zip.Rar](../../aspose.zip.rar/)
* toplantı [Aspose.Zip](../../)


