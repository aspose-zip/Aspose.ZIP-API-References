---
title: Class GzipArchive
second_title: Aspose.ZIP for .NET API Referansı
description: Aspose.Zip.Gzip.GzipArchive sınıf. Bu sınıf gzip arşiv dosyasını temsil eder. Gzip arşivlerini oluşturmak veya çıkarmak için kullanın.
type: docs
weight: 210
url: /tr/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

Bu sınıf, gzip arşiv dosyasını temsil eder. Gzip arşivlerini oluşturmak veya çıkarmak için kullanın.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | Yeni bir örneğini başlatır.`GzipArchive` sıkıştırmak için hazırlanan sınıf. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | Yeni bir örneğini başlatır.`GzipArchive` sıkıştırmayı açmak için hazırlanan sınıf. |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | Yeni bir örneğini başlatır.`GzipArchive` sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | Orijinal dosyanın adı. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | Yönetilmeyen kaynakları serbest bırakma, serbest bırakma veya sıfırlama ile ilişkili uygulama tanımlı görevleri gerçekleştirir. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | Arşivi sağlanan akışa çıkarır. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | Çıkarmak için arşivi açar ve arşiv içeriğine sahip bir akış sağlar. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | Arşivi sağlanan akışa kaydeder. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | Arşivi sağlanan hedef dosyaya kaydeder. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |

### Notlar

Gzip sıkıştırma algoritması, LZ77 ve Huffman kodlamasının bir kombinasyonu olan DEFLATE algoritmasına dayanmaktadır.

### Ayrıca bakınız

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* ad alanı [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* toplantı [Aspose.Zip](../../)


