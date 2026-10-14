---
title: "Sınıf IsoArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Aspose.Zip.Iso.IsoArchive sınıfı. ISO 9660 ISO arşivini temsil eder"
type: docs
weight: 570
url: /tr/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

ISO arşivini (ISO 9660) temsil eder.

```csharp
public sealed class IsoArchive : IArchive
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | Yeni bir `IsoArchive` sınıfı örneği başlatır ve yeni dosya ve dizinler eklemek için boş bir ISO arşivi oluşturur. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | Yeni bir `IsoArchive` sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | Yeni bir `IsoArchive` sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | Arşivi oluşturan [`IsoEntry`](../isoentry/) tipindeki girişleri alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | ISO görüntüsüne bir dizin ekler. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | ISO görüntüsüne bir dosya ekler. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | ISO görüntüsüne bir dosya ekler. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | ISO görüntüsüne bir dosya ekler. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | Yönetilmeyen kaynakların serbest bırakılması, bırakılması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | Tüm girişleri belirtilen dizine çıkarır. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | ISO görüntüsünü belirtilen akışa kaydeder. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | ISO görüntüsünü belirtilen yola kaydeder. |

### Ayrıca Bakınız

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


