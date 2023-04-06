---
title: Class Archive
second_title: Aspose.ZIP for .NET API Referansı
description: Aspose.Zip.Archive sınıf. Bu sınıf zip arşiv dosyasını temsil eder. Zip arşivlerini oluşturmak ayıklamak veya güncellemek için kullanın.
type: docs
weight: 10
url: /tr/net/aspose.zip/archive/
---
## Archive class

Bu sınıf, zip arşiv dosyasını temsil eder. Zip arşivlerini oluşturmak, ayıklamak veya güncellemek için kullanın.

```csharp
public class Archive : IArchive
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | Yeni bir örneğini başlatır.`Archive` girişleri için isteğe bağlı ayarlara sahip sınıf. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | Yeni bir örneğini başlatır.`Archive` class ve composes girişleri listesi arşivden çıkarılabilir. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | Yeni bir örneğini başlatır.`Archive` class ve composes girişleri listesi arşivden çıkarılabilir. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Entries](../../aspose.zip/archive/entries/) { get; } | Şunun girişlerini alır:[`ArchiveEntry`](../archiveentry/) arşivi oluşturan tür. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | Yeni eklenenler için kullanılan sıkıştırma ve şifreleme ayarları[`ArchiveEntry`](../archiveentry/) öğeler. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | Verilen dizindeki tüm dosyaları ve dizinleri tekrar tekrar arşive ekler. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, Stream, ArchiveEntrySettings) | Arşiv içinde tek giriş oluşturun. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, FileInfo, bool, ArchiveEntrySettings) | Arşiv içinde tek giriş oluşturun. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | Arşiv içinde tek giriş oluşturun. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, string, bool, ArchiveEntrySettings) | Arşiv içinde tek giriş oluşturun. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | Belirli bir girişin ilk örneğini girişler listesinden kaldırır. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | Girişi index. ile girişler listesinden kaldırır. |
| [Dispose](../../aspose.zip/archive/dispose/)() | Yönetilmeyen kaynakları serbest bırakma, serbest bırakma veya sıfırlama ile ilişkili uygulama tanımlı görevleri gerçekleştirir. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | Arşivi sağlanan akışa kaydeder. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | Arşivi sağlanan hedef dosyaya kaydeder. |
| [SaveSplit](../../aspose.zip/archive/savesplit/)(string, SplitArchiveSaveOptions) | Çok ciltli arşivi sağlanan hedef dizine kaydeder. |

### Ayrıca bakınız

* interface [IArchive](../iarchive/)
* ad alanı [Aspose.Zip](../../aspose.zip/)
* toplantı [Aspose.Zip](../../)


