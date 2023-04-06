---
title: Class TarArchive
second_title: Aspose.ZIP for .NET API Referansı
description: Aspose.Zip.Tar.TarArchive sınıf. Bu sınıf tar arşiv dosyasını temsil eder. Tar arşivlerini oluşturmak çıkarmak veya güncellemek için kullanın.
type: docs
weight: 730
url: /tr/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Bu sınıf tar arşiv dosyasını temsil eder. Tar arşivlerini oluşturmak, çıkarmak veya güncellemek için kullanın.

```csharp
public class TarArchive : IArchive
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | Yeni bir örneğini başlatır.`TarArchive` sınıf. |
| [TarArchive](tararchive/#constructor_1)(Stream) | Yeni bir örneğini başlatır.[`Archive`](../../aspose.zip/archive/) class ve composes girişleri listesi arşivden çıkarılabilir. |
| [TarArchive](tararchive/#constructor_2)(string) | Yeni bir örneğini başlatır.`TarArchive` class ve composes girişleri listesi arşivden çıkarılabilir. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | Şunun girişlerini alır:[`TarEntry`](../tarentry/) arşivi oluşturan tür. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | Sağlanan gzip arşivini çıkarır ve oluşturur`TarArchive` çıkarılan verilerden. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | Sağlanan gzip arşivini çıkarır ve oluşturur`TarArchive` çıkarılan verilerden. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | Sağlanan lzip arşivini çıkarır ve oluşturur`TarArchive` çıkarılan verilerden. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | Sağlanan lzip arşivini çıkarır ve oluşturur`TarArchive` çıkarılan verilerden. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | Sağlanan xz formatındaki arşivi çıkarır ve oluşturur`TarArchive` çıkarılan verilerden. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | Sağlanan xz formatındaki arşivi çıkarır ve oluşturur`TarArchive` çıkarılan verilerden. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | Sağlanan Z biçimli arşivi çıkarır ve oluşturur`TarArchive` çıkarılan verilerden. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | Sağlanan Z biçimli arşivi çıkarır ve oluşturur`TarArchive` çıkarılan verilerden. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | Arşiv içinde tek giriş oluşturun. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | Arşiv içinde tek giriş oluşturun. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | Arşiv içinde tek giriş oluşturun. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | Girişi index. ile girişler listesinden kaldırır. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | Belirli bir girişin ilk örneğini girişler listesinden kaldırır. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | Yönetilmeyen kaynakları serbest bırakma, serbest bırakma veya sıfırlama ile ilişkili uygulama tanımlı görevleri gerçekleştirir. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | Arşivi sağlanan akışa kaydeder. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | Arşivi sağlanan hedef dosyaya kaydeder. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | Arşivi gzip sıkıştırmasıyla akışa kaydeder. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | Arşivi dosyaya gzip sıkıştırması ile yola göre kaydeder. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | Arşivi lzip sıkıştırmasıyla akışa kaydeder. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | Arşivi, lzip sıkıştırması ile yola göre dosyaya kaydeder. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Arşivi xz sıkıştırmasıyla akışa kaydeder. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Arşivi xz sıkıştırma ile yola göre yola kaydeder. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Arşivi Z sıkıştırmasıyla akışa kaydeder. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Z sıkıştırması ile arşivi yola göre yola kaydeder. |

### Ayrıca bakınız

* interface [IArchive](../../aspose.zip/iarchive/)
* ad alanı [Aspose.Zip.Tar](../../aspose.zip.tar/)
* toplantı [Aspose.Zip](../../)


