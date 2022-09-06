---
title: TarArchive
second_title: Aspose.ZIP for .NET API Referansı
description: Bu sınıf tar arşiv dosyasını temsil eder. Tar arşivlerini oluşturmak ayıklamak veya güncellemek için kullanın.
type: docs
weight: 600
url: /tr/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Bu sınıf, tar arşiv dosyasını temsil eder. Tar arşivlerini oluşturmak, ayıklamak veya güncellemek için kullanın.

```csharp
public class TarArchive : IDisposable
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [TarArchive](tararchive#constructor)() | Yeni bir örneğini başlatır[`TarArchive`](../tararchive) sınıf. |
| [TarArchive](tararchive#constructor_1)(Stream) | Yeni bir örneğini başlatır[`Archive`](../../aspose.zip/archive) sınıf ve oluşturur girdiler listesi arşivden çıkarılabilir. |
| [TarArchive](tararchive#constructor_2)(string) | Yeni bir örneğini başlatır[`TarArchive`](../tararchive) sınıf ve oluşturur girdiler listesi arşivden çıkarılabilir. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries) { get; } | Şunların girişlerini alır:[`TarEntry`](../tarentry) arşivi oluşturan yazın. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip#fromgzip)(Stream) | Sağlanan gzip arşivini çıkarır ve oluşturur[`TarArchive`](../tararchive) çıkarılan verilerden. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip#fromgzip_1)(string) | Sağlanan gzip arşivini çıkarır ve oluşturur[`TarArchive`](../tararchive) çıkarılan verilerden. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip#fromlzip)(Stream) | Sağlanan lzip arşivini çıkarır ve oluşturur[`TarArchive`](../tararchive) çıkarılan verilerden. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip#fromlzip_1)(string) | Sağlanan lzip arşivini çıkarır ve oluşturur[`TarArchive`](../tararchive) çıkarılan verilerden. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz#fromxz)(Stream) | Sağlanan xz formatındaki arşivi çıkarır ve oluşturur[`TarArchive`](../tararchive) çıkarılan verilerden. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz#fromxz_1)(string) | Sağlanan xz formatındaki arşivi çıkarır ve oluşturur[`TarArchive`](../tararchive) çıkarılan verilerden. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz#fromz)(Stream) | Sağlanan Z formatı arşivini çıkarır ve oluşturur[`TarArchive`](../tararchive) çıkarılan verilerden. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz#fromz_1)(string) | Sağlanan Z formatı arşivini çıkarır ve oluşturur[`TarArchive`](../tararchive) çıkarılan verilerden. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries#createentries)(DirectoryInfo, bool) | Verilen dizindeki tüm dosya ve dizinleri yinelemeli olarak arşive ekler. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries#createentries_1)(string, bool) | Verilen dizindeki tüm dosya ve dizinleri yinelemeli olarak arşive ekler. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry#createentry)(string, FileInfo, bool) | Arşiv içinde tek bir giriş oluşturun. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry#createentry_1)(string, Stream, FileSystemInfo) | Arşiv içinde tek bir giriş oluşturun. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry#createentry_2)(string, string, bool) | Arşiv içinde tek bir giriş oluşturun. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry#deleteentry_1)(int) | Girişi, dizine göre giriş listesinden kaldırır. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry#deleteentry)(TarEntry) | Belirli bir girdinin ilk oluşumunu girdiler listesinden kaldırır. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose)() | Yönetilmeyen kaynakları serbest bırakma, serbest bırakma veya sıfırlama ile ilişkili uygulama tanımlı görevleri gerçekleştirir. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory)(string) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |
| [Save](../../aspose.zip.tar/tararchive/save#save)(Stream, TarFormat?) | Arşivi sağlanan akışa kaydeder. |
| [Save](../../aspose.zip.tar/tararchive/save#save_1)(string, TarFormat?) | Arşivi sağlanan hedef dosyaya kaydeder. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped#savegzipped)(Stream, TarFormat?) | Arşivi gzip sıkıştırmasıyla akışa kaydeder. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped#savegzipped_1)(string, TarFormat?) | Arşivi, gzip sıkıştırmasıyla yola göre dosyaya kaydeder. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped#savelzipped)(Stream, TarFormat?) | Arşivi lzip sıkıştırmasıyla akışa kaydeder. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped#savelzipped_1)(string, TarFormat?) | Arşivi lzip sıkıştırmasıyla yola göre dosyaya kaydeder. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Arşivi xz sıkıştırmasıyla akışa kaydeder. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Arşivi, xz sıkıştırmasıyla yola göre kaydeder. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed#savezcompressed)(Stream, TarFormat?) | Arşivi Z sıkıştırmasıyla akışa kaydeder. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed#savezcompressed_1)(string, TarFormat?) | Z sıkıştırmasıyla arşivi yola göre kaydeder. |

### Ayrıca bakınız

* ad alanı [Aspose.Zip.Tar](../../aspose.zip.tar)
* toplantı [Aspose.Zip](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
