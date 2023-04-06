---
title: Class SevenZipArchive
second_title: Aspose.ZIP for .NET API Referansı
description: Aspose.Zip.SevenZip.SevenZipArchive sınıf. Bu sınıf 7z arşiv dosyasını temsil eder. 7z arşivlerini oluşturmak ve çıkarmak için kullanın.
type: docs
weight: 660
url: /tr/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

Bu sınıf, 7z arşiv dosyasını temsil eder. 7z arşivlerini oluşturmak ve çıkarmak için kullanın.

```csharp
public class SevenZipArchive : IArchive
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Yeni bir örneğini başlatır.`SevenZipArchive` girişleri için isteğe bağlı ayarlara sahip sınıf. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | Yeni bir örneğini başlatır.`SevenZipArchive` class ve composes girişleri listesi arşivden çıkarılabilir. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | Yeni bir örneğini başlatır.`SevenZipArchive` class ve composes girişleri listesi arşivden çıkarılabilir. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Şunun girişlerini alır:[`SevenZipArchiveEntry`](../sevenziparchiveentry/) arşivi oluşturan tür. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Yeni eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`SevenZipArchiveEntry`](../sevenziparchiveentry/) öğeler. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | Arşiv içinde tek giriş oluşturun. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | Arşiv içinde tek giriş oluşturun. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Arşiv içinde tek giriş oluşturun. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | Arşiv içinde tek giriş oluşturun. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Yönetilmeyen kaynakları serbest bırakma, serbest bırakma veya sıfırlama ile ilişkili uygulama tanımlı görevleri gerçekleştirir. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | 7z arşivini sağlanan akışa kaydeder. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | Arşivi sağlanan hedef dosyaya kaydeder. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Çok ciltli arşivi sağlanan hedef dizine kaydeder. |

### Ayrıca bakınız

* interface [IArchive](../../aspose.zip/iarchive/)
* ad alanı [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* toplantı [Aspose.Zip](../../)


