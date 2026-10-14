---
title: "Sınıf AppleArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Aspose.Zip.Apple.AppleArchive sınıfı. Bu sınıf bir Apple Archive .aar dosyasını temsil eder. Apple Archive dosyalarını oluşturmak için kullanın."
type: docs
weight: 60
url: /tr/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

Bu sınıf bir Apple Archive (.aar) dosyasını temsil eder. Apple Archive dosyalarını oluşturmak için kullanın.

```csharp
public class AppleArchive : IArchive
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | `AppleArchive` sınıfının yeni bir örneğini, oluşturulan girişler için kullanılan ayarlarla başlatır. |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | `AppleArchive` sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | `AppleArchive` sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | Arşivi oluşturan girişleri alır. |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | Arşivin katı sıkıştırma kullanıp kullanmadığını gösteren bir değer alır. Katı modda, tüm giriş verileri tek bir akış olarak sıkıştırılır ve bireysel giriş çıkarımı mümkün değildir. Bunun yerine [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/) kullanın. |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | Yeni oluşturulan girişler için kullanılan ayarları alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | Verilen dizindeki tüm dosya ve dizinleri, alt dizinler dahil, arşive ekler. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | Arşiv içinde tek bir giriş oluşturur. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | Arşiv içinde tek bir giriş oluşturur. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | Arşiv içinde tek bir giriş oluşturur. |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | Yönetilmeyen kaynakların serbest bırakılması, bırakılması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | Arşivi sağlanan akışa kaydeder. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | Arşivi sağlanan hedef dosyaya kaydeder. |

## Açıklamalar

Apple ve Apple Archive, Apple Inc.'in ticari markalarıdır.

### Ayrıca Bakınız

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


