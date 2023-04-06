---
title: Class CpioArchive
second_title: Aspose.ZIP for .NET API Referansı
description: Aspose.Zip.Cpio.CpioArchive sınıf. Bu sınıf cpio arşiv dosyasını temsil eder.
type: docs
weight: 160
url: /tr/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

Bu sınıf, cpio arşiv dosyasını temsil eder.

```csharp
public class CpioArchive : IArchive
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | Yeni bir örneğini başlatır.`CpioArchive` sınıf. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | Yeni bir örneğini başlatır.`CpioArchive` class ve composes girişleri listesi arşivden çıkarılabilir. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | Yeni bir örneğini başlatır.`CpioArchive` class ve composes girişleri listesi arşivden çıkarılabilir. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | Şunun girişlerini alır:[`CpioEntry`](../cpioentry/) arşivi oluşturan tür. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | Arşiv içinde tek giriş oluşturun. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | Arşiv içinde tek giriş oluşturun. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | Arşiv içinde tek giriş oluşturun. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | Belirli bir girişin ilk örneğini girişler listesinden kaldırır. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | Girişi index. ile girişler listesinden kaldırır. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | Yönetilmeyen kaynakları serbest bırakma, serbest bırakma veya sıfırlama ile ilişkili uygulama tanımlı görevleri gerçekleştirir. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | Arşivi sağlanan akışa kaydeder. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | Arşivi sağlanan hedef dosyaya kaydeder. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | Arşivi gzip sıkıştırmasıyla akışa kaydeder. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | Arşivi dosyaya gzip sıkıştırması ile yola göre kaydeder. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | Arşivi xz sıkıştırmasıyla akışa kaydeder. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | Arşivi xz sıkıştırma ile yola göre yola kaydeder. |

### Ayrıca bakınız

* interface [IArchive](../../aspose.zip/iarchive/)
* ad alanı [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* toplantı [Aspose.Zip](../../)


