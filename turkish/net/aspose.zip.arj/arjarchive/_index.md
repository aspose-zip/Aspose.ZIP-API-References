---
title: "Sınıf ArjArchive"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Aspose.Zip.Arj.ArjArchive sınıfı. Bu sınıf bir ARJ arşiv dosyasını temsil eder."
type: docs
weight: 250
url: /tr/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

Bu sınıf bir ARJ arşiv dosyasını temsil eder.

```csharp
public class ArjArchive : IArchive
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | `ArjArchive` sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | `ArjArchive` sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | Yorumu alır. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | ARJ arşivini oluşturan [`ArjEntryPlain`](../arjentryplain/) tipindeki girişleri alır. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | Orijinal adı alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | Yönetilmeyen kaynakların serbest bırakılması, bırakılması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | Tüm girişleri belirtilen dizine çıkarır. |

## Açıklamalar

Yalnızca aşağıdaki sıkıştırma yöntemleri desteklenir:

**Method**

**Explanation**

**0**

Sıkıştırılmamış

**1**

LZ77 ve uyarlamalı Huffman kodlamasının kombinasyonu. En iyi oran.

**2**

LZ77 ve uyarlamalı Huffman kodlamasının kombinasyonu.

**3**

LZ77 ve uyarlamalı Huffman kodlamasının kombinasyonu. En hızlı.

### Ayrıca Bakınız

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


